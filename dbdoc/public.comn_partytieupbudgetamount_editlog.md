# public.comn_partytieupbudgetamount_editlog

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| logdetailid | integer | nextval('comn_partytieupbudgetamount_editlog_logdetailid_seq'::regclass) | false |  |  |  |
| branchid | integer |  | true |  |  |  |
| finyearid | integer |  | true |  |  |  |
| finyear | text |  | true |  |  |  |
| startdate | date |  | true |  |  |  |
| enddate | date |  | true |  |  |  |
| partyid | integer |  | true |  |  |  |
| amount | numeric(21,9) |  | true |  |  |  |
| createdon | timestamp(6) without time zone | now() | true |  |  |  |
| createdby | integer |  | true |  |  |  |
| isauthorized | boolean | false | true |  |  |  |
| authorizedby | integer |  | true |  |  |  |
| authorizedon | timestamp(6) without time zone | now() | true |  |  |  |
| iscancelled | boolean | false | true |  |  |  |
| cancelledby | integer |  | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| pkey_partytieupbudgetamount_editlog | PRIMARY KEY | PRIMARY KEY (logdetailid) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| pkey_partytieupbudgetamount_editlog | CREATE UNIQUE INDEX pkey_partytieupbudgetamount_editlog ON public.comn_partytieupbudgetamount_editlog USING btree (logdetailid) |

## Relations

![er](public.comn_partytieupbudgetamount_editlog.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)
