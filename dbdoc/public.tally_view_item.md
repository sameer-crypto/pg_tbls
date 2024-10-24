# public.tally_view_item

## Description

<details>
<summary><strong>Table Definition</strong></summary>

```sql
CREATE VIEW tally_view_item AS (
 SELECT itm.itemid,
    COALESCE(itm.nameintally, itm.itemname) AS itemname,
    itm.itemcode,
    itm.drawingno,
    itm.itemcategory,
    itm.unitid,
    bunit.noofdecimalplace AS basedecimalplaces,
    bunit.shortname AS baseunit,
    itm.revisionno,
    itm.issueno,
    COALESCE(itm.tally_purchase_ledger, stor_itemgroup.tally_purchase_ledger) AS purchase_ledger,
    COALESCE(itm.tally_sales_ledger, stor_itemgroup.tally_sales_ledger) AS sales_ledger,
    COALESCE(itm.conversion, (0)::numeric) AS conversion,
    itm.altunitid,
    itm.denominator,
    aunit.noofdecimalplace AS altdecimalplaces,
    aunit.shortname AS altunit,
    itm.isbomnotrequiredforproduction,
    itm.field1,
    itm.description,
    COALESCE(itm.isserialonaltunit, false) AS isserialonaltunit,
    COALESCE(itm.isbatchonaltunit, false) AS isbatchonaltunit,
        CASE
            WHEN (itm.isenableseries IS NULL) THEN false
            ELSE itm.isenableseries
        END AS isenableseries,
    itm.isinspectionrequired,
    itm.isenablebatchcreation,
    itm.groupid,
    itm.printname,
    COALESCE(itm.cstrate, (0)::numeric) AS cstrate,
    COALESCE(itm.vatrate, (0)::numeric) AS vatrate,
    pack.shortname AS packingunit,
    itm.packsizeof,
    itm.exciseclassificationid,
    stor_itemgroup.groupname,
    COALESCE(itm.isusedasacapitalgoods, false) AS isusedasacapitalgoods,
    itm.isactive
   FROM ((((stor_itemmaster itm
     LEFT JOIN stor_measurementunit bunit ON ((itm.unitid = bunit.unitid)))
     LEFT JOIN stor_measurementunit aunit ON ((itm.altunitid = aunit.unitid)))
     LEFT JOIN stor_measurementunit pack ON ((itm.packinguomid = pack.unitid)))
     LEFT JOIN stor_itemgroup ON ((itm.groupid = stor_itemgroup.groupid)))
)
```

</details>

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| itemid | integer |  | true |  |  |  |
| itemname | varchar(200) |  | true |  |  |  |
| itemcode | varchar(50) |  | true |  |  |  |
| drawingno | varchar(50) |  | true |  |  |  |
| itemcategory | smallint |  | true |  |  |  |
| unitid | integer |  | true |  |  |  |
| basedecimalplaces | smallint |  | true |  |  |  |
| baseunit | varchar(10) |  | true |  |  |  |
| revisionno | integer |  | true |  |  |  |
| issueno | integer |  | true |  |  |  |
| purchase_ledger | text |  | true |  |  |  |
| sales_ledger | text |  | true |  |  |  |
| conversion | numeric |  | true |  |  |  |
| altunitid | integer |  | true |  |  |  |
| denominator | numeric(16,6) |  | true |  |  |  |
| altdecimalplaces | smallint |  | true |  |  |  |
| altunit | varchar(10) |  | true |  |  |  |
| isbomnotrequiredforproduction | boolean |  | true |  |  |  |
| field1 | varchar(50) |  | true |  |  |  |
| description | varchar(1000) |  | true |  |  |  |
| isserialonaltunit | boolean |  | true |  |  |  |
| isbatchonaltunit | boolean |  | true |  |  |  |
| isenableseries | boolean |  | true |  |  |  |
| isinspectionrequired | boolean |  | true |  |  |  |
| isenablebatchcreation | boolean |  | true |  |  |  |
| groupid | integer |  | true |  |  |  |
| printname | varchar(200) |  | true |  |  |  |
| cstrate | numeric |  | true |  |  |  |
| vatrate | numeric |  | true |  |  |  |
| packingunit | varchar(10) |  | true |  |  |  |
| packsizeof | numeric(14,4) |  | true |  |  |  |
| exciseclassificationid | integer |  | true |  |  |  |
| groupname | varchar(100) |  | true |  |  |  |
| isusedasacapitalgoods | boolean |  | true |  |  |  |
| isactive | boolean |  | true |  |  |  |

## Referenced Tables

| Name | Columns | Comment | Type |
| ---- | ------- | ------- | ---- |
| [public.stor_itemmaster](public.stor_itemmaster.md) | 178 |  | BASE TABLE |
| [public.stor_measurementunit](public.stor_measurementunit.md) | 25 |  | BASE TABLE |
| [public.stor_itemgroup](public.stor_itemgroup.md) | 36 |  | BASE TABLE |

## Relations

![er](public.tally_view_item.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)
