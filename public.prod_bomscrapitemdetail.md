# public.prod_bomscrapitemdetail

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| bomscrapdetailid | integer | nextval('prod_bomscrapitemdetail_bomscrapdetailid_seq'::regclass) | false |  |  |  |
| bomid | integer |  | true |  |  |  |
| itemid | integer |  | true |  |  |  |
| scrapbaseqty | numeric(15,5) |  | true |  |  |  |
| scrapaltqty | numeric(15,5) |  | true |  |  |  |
| toleranceplus | numeric(10,2) |  | true |  |  |  |
| toleranceminus | numeric(10,2) |  | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| prod_bomscrapitemdetail_pkey | PRIMARY KEY | PRIMARY KEY (bomscrapdetailid) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| prod_bomscrapitemdetail_pkey | CREATE UNIQUE INDEX prod_bomscrapitemdetail_pkey ON public.prod_bomscrapitemdetail USING btree (bomscrapdetailid) |

## Relations

![er](public.prod_bomscrapitemdetail.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)