# public.sale_sobatchdetail_proforma

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| sobatchdetailid | integer | nextval('sale_sobatchdetail_proforma_sobatchdetailid_seq'::regclass) | false |  |  |  |
| soid | integer |  | true |  |  |  |
| sodetailid | integer |  | true |  |  |  |
| itemid | integer |  | true |  |  |  |
| batchid | integer |  | true |  |  |  |
| batchholdbaseqty | numeric(15,5) |  | true |  |  |  |
| batchholdaltqty | numeric(15,5) |  | true |  |  |  |
| proforma_id | integer | 0 | true |  |  |  |
| proformadetail_id | integer | 0 | true |  |  |  |
| rackid | integer | 0 | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| sale_sobatchdetail_proforma_pkey | PRIMARY KEY | PRIMARY KEY (sobatchdetailid) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| sale_sobatchdetail_proforma_pkey | CREATE UNIQUE INDEX sale_sobatchdetail_proforma_pkey ON public.sale_sobatchdetail_proforma USING btree (sobatchdetailid) |

## Relations

![er](public.sale_sobatchdetail_proforma.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)
