# public.stor_storeissuefielddetail

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| issuefielddetailid | integer | nextval('stor_storeissuefielddetail_issuefielddetailid_seq'::regclass) | false |  |  |  |
| issueid | integer |  | true |  |  |  |
| fieldid | integer |  | true |  |  |  |
| fieldvalue | text |  | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| stor_storeissuefielddetail_pkey | PRIMARY KEY | PRIMARY KEY (issuefielddetailid) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| stor_storeissuefielddetail_pkey | CREATE UNIQUE INDEX stor_storeissuefielddetail_pkey ON public.stor_storeissuefielddetail USING btree (issuefielddetailid) |

## Relations

![er](public.stor_storeissuefielddetail.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)