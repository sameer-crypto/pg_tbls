# public.prod_batchcardserialdetail

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| batchcardserialid | integer | nextval('prod_batchcardserialdetail_batchcardserialid_seq'::regclass) | false |  |  |  |
| batchcardid | integer |  | true |  |  |  |
| batchid | integer |  | true |  |  |  |
| serialid | bigint |  | true |  |  |  |
| productiondetialid | integer |  | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| prod_batchcardserialdetail_pkey | PRIMARY KEY | PRIMARY KEY (batchcardserialid) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| prod_batchcardserialdetail_pkey | CREATE UNIQUE INDEX prod_batchcardserialdetail_pkey ON public.prod_batchcardserialdetail USING btree (batchcardserialid) |

## Relations

![er](public.prod_batchcardserialdetail.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)
