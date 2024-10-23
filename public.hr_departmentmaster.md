# public.hr_departmentmaster

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| departmentid | integer | nextval('hr_departmentmaster_departmentid_seq'::regclass) | false |  |  |  |
| department | varchar(100) |  | false |  |  |  |
| isactive | boolean | false | false |  |  |  |
| isauthorized | boolean | false | false |  |  |  |
| authorizedby | integer |  | true |  |  |  |
| authorizedon | timestamp without time zone |  | true |  |  |  |
| createdby | integer |  | true |  |  |  |
| createdon | timestamp without time zone | now() | true |  |  |  |
| editlog | text |  | true |  |  |  |
| headauthorizedby | integer |  | true |  |  |  |
| headauthorizedon | timestamp without time zone |  | true |  |  |  |
| short_name | varchar(100) |  | true |  |  |  |
| description | varchar(1000) |  | true |  |  |  |
| inactivedate | timestamp without time zone |  | true |  |  |  |
| lastmodifiedon | timestamp(6) without time zone | now() | true |  |  |  |
| updatedby | integer |  | true |  |  |  |
| updatedon | timestamp(6) without time zone | NULL::timestamp without time zone | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| departmentmaster_department_key | UNIQUE | UNIQUE (department) |
| departmentmaster_pkey | PRIMARY KEY | PRIMARY KEY (departmentid) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| departmentmaster_department_key | CREATE UNIQUE INDEX departmentmaster_department_key ON public.hr_departmentmaster USING btree (department) |
| departmentmaster_pkey | CREATE UNIQUE INDEX departmentmaster_pkey ON public.hr_departmentmaster USING btree (departmentid) |

## Relations

![er](public.hr_departmentmaster.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)