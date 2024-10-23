# scheme.scheme_range_period_detail

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| scheme_id | integer |  | true |  |  |  |
| partycode | varchar(50) |  | true |  |  |  |
| period_id | integer |  | true |  |  |  |
| range_id | integer |  | true |  |  |  |
| range_no | varchar(150) |  | true |  |  |  |
| period_name | varchar(50) |  | true |  |  |  |
| isforevery | boolean |  | true |  |  |  |
| quantity | numeric(12,2) |  | true |  |  |  |
| volume | numeric(12,2) |  | true |  |  |  |
| amount | numeric(12,2) |  | true |  |  |  |
| slab_name | varchar(50) |  | true |  |  |  |
| slab_id | integer |  | true |  |  |  |
| cn_value | numeric(12,2) |  | true |  |  |  |
| cn_rate | numeric(5,2) |  | true |  |  |  |
| for_every_rate | numeric(10,2) |  | true |  |  |  |
| points | integer |  | true |  |  |  |
| result_value | numeric(12,2) |  | true |  |  |  |
| gift | text |  | true |  |  |  |
| slab_no | integer |  | true |  |  |  |

## Relations

![er](scheme.scheme_range_period_detail.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)