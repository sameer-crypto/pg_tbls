# public.comn_serialmapping

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| trnid | integer | nextval('comn_serialmapping_trnid_seq'::regclass) | false |  |  |  |
| trndate | date |  | true |  |  |  |
| trnno | varchar |  | true |  |  |  |
| scanvalue1 | text |  | true |  |  |  |
| branchid | integer |  | true |  |  |  |
| createdby | integer |  | false |  |  |  |
| isauthorized | boolean | false | false |  |  |  |
| iscancelled | boolean | false | false |  |  |  |
| authorizedby | integer |  | true |  |  |  |
| authorizedon | timestamp(6) without time zone |  | true |  |  |  |
| seriescode | varchar(50) |  | true |  |  |  |
| seriesno | integer |  | true |  |  |  |
| editlog | text |  | true |  |  |  |
| createdon | timestamp(6) without time zone | now() | true |  |  |  |
| amendby | integer |  | true |  |  |  |
| amendon | date |  | true |  |  |  |
| seriesvouchertype | smallint | 0 | true |  |  |  |
| seriesid | integer |  | true |  |  |  |
| amendreason | text |  | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| comn_serialmapping_pkey | PRIMARY KEY | PRIMARY KEY (trnid) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| comn_serialmapping_pkey | CREATE UNIQUE INDEX comn_serialmapping_pkey ON public.comn_serialmapping USING btree (trnid) |

## Relations

![er](public.comn_serialmapping.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)