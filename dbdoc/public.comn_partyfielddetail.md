# public.comn_partyfielddetail

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| partyfielddetailid | integer | nextval('comn_partyfielddetail_partyfielddetailid_seq'::regclass) | false |  |  |  |
| partyid | integer |  | true |  |  |  |
| fieldid | integer |  | true |  |  |  |
| fieldvalue | text |  | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| comn_partyfielddetail_pkey | PRIMARY KEY | PRIMARY KEY (partyfielddetailid) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| comn_partyfielddetail_pkey | CREATE UNIQUE INDEX comn_partyfielddetail_pkey ON public.comn_partyfielddetail USING btree (partyfielddetailid) |

## Relations

![er](public.comn_partyfielddetail.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)
