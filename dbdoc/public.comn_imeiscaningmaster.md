# public.comn_imeiscaningmaster

## Description

IMEI Scanning entry master after Gate Entry and before Inward challan

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| imeiscanningid | integer | nextval('comn_imeiscaningmaster_imeiscanningid_seq'::regclass) | false |  |  |  |
| entryno | varchar(50) |  | true |  |  |  |
| entrydate | timestamp without time zone |  | true |  |  |  |
| gateentryid | integer |  | true |  |  |  |
| gateentryimeidetailid | integer |  | true |  |  |  |
| branchid | integer |  | true |  |  |  |
| createdby | integer |  | true |  |  |  |
| createdon | timestamp without time zone | now() | true |  |  |  |
| isauthorized | boolean | false | false |  |  |  |
| authorizedon | timestamp without time zone |  | true |  |  |  |
| authorizedby | integer |  | true |  |  |  |
| iscancelled | boolean |  | true |  |  |  |
| seriesno | integer |  | true |  |  |  |
| seriescode | varchar(50) |  | true |  |  |  |
| seriesid | integer |  | true |  |  |  |
| seriesvouchertype | smallint | 0 | true |  |  |  |
| editlog | text |  | true |  |  |  |
| headauthorizedby | integer |  | true |  |  |  |
| headauthorizedon | timestamp without time zone |  | true |  |  |  |
| updatedby | integer |  | true |  |  |  |
| updatedon | timestamp(6) without time zone | NULL::timestamp without time zone | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| comn_imeiscaningmaster_pkey | PRIMARY KEY | PRIMARY KEY (imeiscanningid) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| comn_imeiscaningmaster_pkey | CREATE UNIQUE INDEX comn_imeiscaningmaster_pkey ON public.comn_imeiscaningmaster USING btree (imeiscanningid) |

## Relations

![er](public.comn_imeiscaningmaster.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)
