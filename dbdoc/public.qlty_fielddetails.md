# public.qlty_fielddetails

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| tifielddetailid | integer | nextval('qlty_fielddetails_tifielddetailid_seq'::regclass) | false |  |  |  |
| tiid | integer |  | true |  |  |  |
| fieldid | integer |  | true |  |  |  |
| fieldvalue | varchar(200) |  | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| qlty_fielddetails_pkey | PRIMARY KEY | PRIMARY KEY (tifielddetailid) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| qlty_fielddetails_pkey | CREATE UNIQUE INDEX qlty_fielddetails_pkey ON public.qlty_fielddetails USING btree (tifielddetailid) |

## Relations

![er](public.qlty_fielddetails.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)
