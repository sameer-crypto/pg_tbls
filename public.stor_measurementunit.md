# public.stor_measurementunit

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| unitid | integer | nextval('stor_measurementunit_unitid_seq'::regclass) | false | [public.stor_itemmaster](public.stor_itemmaster.md) [public.prod_scrapmaster](public.prod_scrapmaster.md) |  |  |
| unitname | varchar(20) |  | true |  |  |  |
| shortname | varchar(10) |  | true |  |  |  |
| noofdecimalplace_old | numeric(1,0) |  | true |  |  |  |
| issendtotelly | boolean | false | true |  |  |  |
| isactive | boolean | true | false |  |  |  |
| isauthorized | boolean | false | false |  |  |  |
| authorizedon | timestamp without time zone |  | true |  |  |  |
| authorizedby | integer |  | true |  |  |  |
| createdby | integer |  | true |  |  |  |
| editlog | text |  | true |  |  |  |
| createdon | timestamp without time zone | now() | true |  |  |  |
| headauthorizedon | timestamp without time zone |  | true |  |  |  |
| headauthorizedby | integer |  | true |  |  |  |
| noofdecimalplace | smallint | 0 | true |  |  |  |
| sentincrm | boolean | false | true |  |  |  |
| alterid | integer |  | true |  |  |  |
| calculationvalueforapiinbom | numeric(21,3) | 0 | false |  |  |  |
| iscalculateinpercentageinbom | boolean | false | false |  |  |  |
| unitquantitycodeid | integer | 0 | false |  |  |  |
| globalname | varchar(20) | ''::character varying | true |  |  |  |
| lastmodifiedon | timestamp(6) without time zone | now() | true |  |  |  |
| updatedby | integer |  | true |  |  |  |
| updatedon | timestamp(6) without time zone | NULL::timestamp without time zone | true |  |  |  |
| inputformula | text | ''::text | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| measurementunit_pkey | PRIMARY KEY | PRIMARY KEY (unitid) |
| measurementunit_shortname_key | UNIQUE | UNIQUE (shortname) |
| measurementunit_unitname_key | UNIQUE | UNIQUE (unitname) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| measurementunit_pkey | CREATE UNIQUE INDEX measurementunit_pkey ON public.stor_measurementunit USING btree (unitid) |
| measurementunit_shortname_key | CREATE UNIQUE INDEX measurementunit_shortname_key ON public.stor_measurementunit USING btree (shortname) |
| measurementunit_unitname_key | CREATE UNIQUE INDEX measurementunit_unitname_key ON public.stor_measurementunit USING btree (unitname) |
| Index_Unit_AlUnitID | CREATE INDEX "Index_Unit_AlUnitID" ON public.stor_measurementunit USING btree (alterid) |

## Triggers

| Name | Definition |
| ---- | ---------- |
| trg_unitalterid | CREATE TRIGGER trg_unitalterid AFTER INSERT OR UPDATE ON public.stor_measurementunit FOR EACH ROW EXECUTE FUNCTION updatealterid() |

## Relations

![er](public.stor_measurementunit.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)