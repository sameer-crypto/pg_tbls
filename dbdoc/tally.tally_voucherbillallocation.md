# tally.tally_voucherbillallocation

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| tallyvoucherbillallocationid | integer | nextval('tally.tally_voucherbillallocation_tallyvoucherbillallocationid_seq'::regclass) | false |  |  |  |
| vouchermasterid | integer |  | true |  |  |  |
| tallyvoucherdetailid | integer |  | true |  |  |  |
| billtype | varchar(100) |  | true |  |  |  |
| billname | varchar(200) |  | true |  |  |  |
| amount | numeric(15,5) |  | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| tally_voucherbillallocation_pkey | PRIMARY KEY | PRIMARY KEY (tallyvoucherbillallocationid) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| tally_voucherbillallocation_pkey | CREATE UNIQUE INDEX tally_voucherbillallocation_pkey ON tally.tally_voucherbillallocation USING btree (tallyvoucherbillallocationid) |

## Relations

![er](tally.tally_voucherbillallocation.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)