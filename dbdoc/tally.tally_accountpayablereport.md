# tally.tally_accountpayablereport

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| detailid | integer | nextval('tally.tally_accountpayablereport_detailid_seq'::regclass) | false |  |  |  |
| ledgername | varchar(300) |  | true |  |  |  |
| outstandingamt | numeric(15,5) | 0 | true |  |  |  |
| amounttype | varchar(20) |  | true |  |  |  |
| branchid | integer |  | true |  |  |  |
| tallybookname | varchar(300) |  | true |  |  |  |
| billdate | date |  | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| tally_accountpayablereport_pkey | PRIMARY KEY | PRIMARY KEY (detailid) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| tally_accountpayablereport_pkey | CREATE UNIQUE INDEX tally_accountpayablereport_pkey ON tally.tally_accountpayablereport USING btree (detailid) |

## Relations

![er](tally.tally_accountpayablereport.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)
