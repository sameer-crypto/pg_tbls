# public.qlty_iaminspectionparameter

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| parameterdetailid | integer | nextval('qlty_iaminspectionparameter_parameterdetailid_seq'::regclass) | false |  |  |  |
| inspectionid | integer |  | true |  |  |  |
| inspectiondetailid | integer |  | true |  |  |  |
| qltyparameterid | integer |  | true |  |  |  |
| value | numeric(10,4) |  | true |  |  |  |
| itemparameterdetailid | integer |  | true |  |  |  |
| remarks | text |  | true |  |  |  |
| paramtext | text |  | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| qlty_iaminspectionparameter_pkey | PRIMARY KEY | PRIMARY KEY (parameterdetailid) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| qlty_iaminspectionparameter_pkey | CREATE UNIQUE INDEX qlty_iaminspectionparameter_pkey ON public.qlty_iaminspectionparameter USING btree (parameterdetailid) |
| Index_IAM_ParmDet_DetID | CREATE INDEX "Index_IAM_ParmDet_DetID" ON public.qlty_iaminspectionparameter USING btree (inspectiondetailid) |
| Index_IAM_ParmDet_IAMIDDetID | CREATE INDEX "Index_IAM_ParmDet_IAMIDDetID" ON public.qlty_iaminspectionparameter USING btree (inspectionid, inspectiondetailid) |

## Relations

![er](public.qlty_iaminspectionparameter.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)
