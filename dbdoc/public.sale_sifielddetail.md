# public.sale_sifielddetail

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| sifielddetailid | integer | nextval('sale_sifielddetail_sifielddetailid_seq'::regclass) | false |  |  |  |
| siid | integer |  | true |  |  |  |
| fieldid | integer |  | true |  |  |  |
| fieldvalue | text |  | true |  |  |  |
| fieldcaption | text |  | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| sale_sifielddetail_pkey | PRIMARY KEY | PRIMARY KEY (sifielddetailid) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| sale_sifielddetail_pkey | CREATE UNIQUE INDEX sale_sifielddetail_pkey ON public.sale_sifielddetail USING btree (sifielddetailid) |
| Index_SI_FielDet_SIID | CREATE INDEX "Index_SI_FielDet_SIID" ON public.sale_sifielddetail USING btree (siid) |

## Relations

![er](public.sale_sifielddetail.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)
