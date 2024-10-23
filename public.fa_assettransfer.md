# public.fa_assettransfer

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| assettransferid | integer | nextval('fa_assettransfer_assettransferid_seq'::regclass) | false |  |  |  |
| assettransferno | varchar(20) |  | true |  |  |  |
| transferedby | integer |  | true |  |  |  |
| transferedon | date |  | true |  |  |  |
| authorizedby | integer |  | true |  |  |  |
| authorizedon | timestamp without time zone |  | true |  |  |  |
| createdby | integer |  | true |  |  |  |
| createdon | timestamp without time zone | now() | true |  |  |  |
| editlog | text |  | true |  |  |  |
| isauthorized | boolean | false | true |  |  |  |
| seriesid | integer |  | true |  |  |  |
| seriesno | integer |  | true |  |  |  |
| iscancelled | boolean | false | false |  |  |  |
| branchid | integer | 0 | false |  |  |  |
| updatedby | integer |  | true |  |  |  |
| updatedon | timestamp(6) without time zone | NULL::timestamp without time zone | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| fa_assettransfer_pkey1 | PRIMARY KEY | PRIMARY KEY (assettransferid) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| fa_assettransfer_pkey1 | CREATE UNIQUE INDEX fa_assettransfer_pkey1 ON public.fa_assettransfer USING btree (assettransferid) |

## Relations

![er](public.fa_assettransfer.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)