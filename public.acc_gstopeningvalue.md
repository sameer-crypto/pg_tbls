# public.acc_gstopeningvalue

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| openingid | integer | nextval('acc_gstopeningvalue_openingid_seq'::regclass) | false |  |  |  |
| exciseclassificationid | integer | 0 | false |  |  |  |
| igstamount | numeric(15,2) | 0 | false |  |  |  |
| cgstamount | numeric(15,2) | 0 | false |  |  |  |
| sgstamount | numeric(15,2) | 0 | false |  |  |  |
| cessamount | numeric(15,2) | 0 | false |  |  |  |
| branchid | integer |  | true |  |  |  |
| createdby | integer | 0 | false |  |  |  |
| createdon | timestamp(6) without time zone |  | true |  |  |  |
| isauthorized | boolean | false | false |  |  |  |
| authorizedby | integer |  | true |  |  |  |
| authorizedon | timestamp(6) without time zone |  | true |  |  |  |
| editlog | text |  | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| acc_gstopeningvalue_pkey | PRIMARY KEY | PRIMARY KEY (openingid) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| acc_gstopeningvalue_pkey | CREATE UNIQUE INDEX acc_gstopeningvalue_pkey ON public.acc_gstopeningvalue USING btree (openingid) |

## Relations

![er](public.acc_gstopeningvalue.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)