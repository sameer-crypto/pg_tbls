# public.pay_attendance_withoutleave_details

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| attendancewoutldetailsid | integer | nextval('pay_attendance_withoutleave_detail_attendancewoutldetailsid_seq'::regclass) | false |  |  |  |
| attendancewoutlmasterid | integer |  | true |  |  |  |
| employeeid | integer |  | true |  |  |  |
| noofdayswoutpl | numeric(18,2) |  | true |  |  |  |
| monthdays | integer |  | true |  |  |  |
| payabledays | numeric(18,2) |  | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| pay_attendance_withoutleave_details_pkey | PRIMARY KEY | PRIMARY KEY (attendancewoutldetailsid) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| pay_attendance_withoutleave_details_pkey | CREATE UNIQUE INDEX pay_attendance_withoutleave_details_pkey ON public.pay_attendance_withoutleave_details USING btree (attendancewoutldetailsid) |

## Relations

![er](public.pay_attendance_withoutleave_details.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)
