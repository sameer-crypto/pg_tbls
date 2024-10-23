# public.pur_pifielddetail

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| pifielddetailid | integer | nextval('pur_pifielddetail_pifielddetailid_seq'::regclass) | false |  |  |  |
| piid | integer |  | true |  |  |  |
| fieldid | integer |  | true |  |  |  |
| fieldvalue | text |  | true |  |  |  |
| fieldcaption | text |  | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| pur_pifielddetail_pkey | PRIMARY KEY | PRIMARY KEY (pifielddetailid) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| pur_pifielddetail_pkey | CREATE UNIQUE INDEX pur_pifielddetail_pkey ON public.pur_pifielddetail USING btree (pifielddetailid) |
| Index_PI_FielDet_PIID | CREATE INDEX "Index_PI_FielDet_PIID" ON public.pur_pifielddetail USING btree (piid) |

## Relations

![er](public.pur_pifielddetail.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)