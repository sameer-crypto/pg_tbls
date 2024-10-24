# public.prod_costsheetdetail

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| sheetdetailid | integer | nextval('prod_costsheetdetail_sheetdetailid_seq'::regclass) | false |  |  |  |
| sheetid | integer |  | true |  |  |  |
| fieldcode | varchar(50) |  | true |  |  |  |
| fieldname | varchar(250) |  | true |  |  |  |
| fieldtype | smallint |  | true |  |  |  |
| isvisible | boolean |  | true |  |  |  |
| fieldvaluefrom | smallint |  | true |  |  |  |
| fieldvalue | varchar(250) |  | true |  |  |  |
| seq_no | smallint |  | true |  |  |  |
| isnumeric | boolean |  | true |  |  |  |
| field_width | smallint | 70 | true |  |  |  |
| isprint | boolean | false | true |  |  |  |
| itemgroupid | integer | 0 | true |  |  |  |
| iseditable | boolean | true | true |  |  |  |
| noofdecimalplace | numeric(18,0) | 2 | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| prod_costsheetdetail_pkey | PRIMARY KEY | PRIMARY KEY (sheetdetailid) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| prod_costsheetdetail_pkey | CREATE UNIQUE INDEX prod_costsheetdetail_pkey ON public.prod_costsheetdetail USING btree (sheetdetailid) |

## Triggers

| Name | Definition |
| ---- | ---------- |
| costsheetmaster_amend_log_entry | CREATE TRIGGER costsheetmaster_amend_log_entry BEFORE UPDATE ON public.prod_costsheetdetail FOR EACH ROW EXECUTE FUNCTION costsheetmaster_amend_log_entry() |

## Relations

![er](public.prod_costsheetdetail.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)
