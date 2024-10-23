# public.log_storesummeryreport_log

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| tableid | integer | nextval('log_storesummeryreport_log_tableid_seq'::regclass) | false |  |  |  |
| entryid | bigint |  | true |  |  |  |
| entryno | varchar(250) |  | true |  |  |  |
| entrydate | date |  | true |  |  |  |
| branchid | integer |  | true |  |  |  |
| entryidtype | varchar(250) |  | true |  |  |  |
| remarks | varchar(250) |  | true |  |  |  |
| createdon | timestamp without time zone |  | true |  |  |  |
| createdby | integer |  | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| log_storesummeryreport_log_pkey | PRIMARY KEY | PRIMARY KEY (tableid) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| log_storesummeryreport_log_pkey | CREATE UNIQUE INDEX log_storesummeryreport_log_pkey ON public.log_storesummeryreport_log USING btree (tableid) |

## Relations

![er](public.log_storesummeryreport_log.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)