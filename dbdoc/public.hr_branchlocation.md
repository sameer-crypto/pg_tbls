# public.hr_branchlocation

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| un_id | integer | nextval('hr_branchlocation_un_id_seq'::regclass) | false |  |  |  |
| branchid | integer |  | false |  |  |  |
| locationid | integer |  | false |  |  |  |
| isactive | boolean |  | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| hr_branchlocation_pkey | PRIMARY KEY | PRIMARY KEY (un_id) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| hr_branchlocation_pkey | CREATE UNIQUE INDEX hr_branchlocation_pkey ON public.hr_branchlocation USING btree (un_id) |

## Relations

![er](public.hr_branchlocation.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)
