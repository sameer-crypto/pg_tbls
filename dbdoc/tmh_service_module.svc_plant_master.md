# tmh_service_module.svc_plant_master

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| plant_id | integer | nextval('tmh_service_module.svc_plant_master_plant_id_seq'::regclass) | false |  |  |  |
| plant_name | varchar(30) |  | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| svc_plant_master_pkey | PRIMARY KEY | PRIMARY KEY (plant_id) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| svc_plant_master_pkey | CREATE UNIQUE INDEX svc_plant_master_pkey ON tmh_service_module.svc_plant_master USING btree (plant_id) |

## Relations

![er](tmh_service_module.svc_plant_master.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)
