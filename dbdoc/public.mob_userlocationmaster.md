# public.mob_userlocationmaster

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| locationid | integer | nextval('mob_userlocationmaster_locationid_seq'::regclass) | false |  |  |  |
| alterid | bigint |  | true |  |  |  |
| emp_id | text |  | true |  |  |  |
| client_id | integer |  | true |  |  |  |
| other_client_id | bigint |  | true |  |  |  |
| start_date | timestamp without time zone |  | true |  |  |  |
| end_date | timestamp without time zone |  | true |  |  |  |
| longitude | text |  | true |  |  |  |
| latitude | text |  | true |  |  |  |
| isactive | boolean |  | true |  |  |  |
| delflag | boolean |  | true |  |  |  |
| created_by | text |  | true |  |  |  |
| created_on | timestamp without time zone | now() | true |  |  |  |
| locationmasterid | integer |  | true |  |  |  |
| locationtype | integer |  | true |  |  |  |

## Relations

![er](public.mob_userlocationmaster.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)
