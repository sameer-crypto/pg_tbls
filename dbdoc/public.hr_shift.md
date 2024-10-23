# public.hr_shift

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| shiftid | integer | nextval('hr_shift_shiftid_seq'::regclass) | false |  |  |  |
| shiftname | varchar(30) |  | true |  |  |  |
| description | varchar(50) |  | true |  |  |  |
| isactive | boolean | false | false |  |  |  |
| isauthorized | boolean | false | false |  |  |  |
| starttime | timestamp without time zone |  | true |  |  |  |
| endtime | timestamp without time zone |  | true |  |  |  |
| branchid | smallint |  | true |  |  |  |
| authorizedby | integer |  | true |  |  |  |
| authorizedon | timestamp without time zone |  | true |  |  |  |
| applicablefrom | date |  | true |  |  |  |
| editlog | text |  | true |  |  |  |
| createdby | integer |  | true |  |  |  |
| createdon | timestamp without time zone | now() | true |  |  |  |
| shiftshortname | varchar(5) |  | true |  |  |  |
| headauthorizedby | integer |  | true |  |  |  |
| headauthorizedon | timestamp without time zone |  | true |  |  |  |
| inactivedate | timestamp without time zone |  | true |  |  |  |
| updatedby | integer |  | true |  |  |  |
| updatedon | timestamp(6) without time zone | NULL::timestamp without time zone | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| hr_shift_pkey | PRIMARY KEY | PRIMARY KEY (shiftid) |
| shiftname | UNIQUE | UNIQUE (shiftname, branchid) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| hr_shift_pkey | CREATE UNIQUE INDEX hr_shift_pkey ON public.hr_shift USING btree (shiftid) |
| shiftname | CREATE UNIQUE INDEX shiftname ON public.hr_shift USING btree (shiftname, branchid) |

## Relations

![er](public.hr_shift.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)