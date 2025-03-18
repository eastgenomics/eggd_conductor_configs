## 📄 Uranus input files

Below defines all external input files, their versions and file locations in DNAnexus used as part of the Uranus pipeline. These are used in the eggd_conductor assay config file within the `inputs` section for each executable

---
### [Uranus main workflow](https://github.com/eastgenomics/eggd_uranus_main_workflow)

| App 	| Input field |  Input file 	| Version  	|
|---	|---	|---	|--- |
|[cgppindel](https://github.com/eastgenomics/eggd_cgppindel)| `normal` |[TA2_S59_L008_tumor_markdup_nochr.bam](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/?scope=project&id.values=file-GjQGgXQ4qv8QF2FFVqYQJj5J)|not versioned|
||`normal_index`|[TA2_S59_L008_tumor_markdup_nochr.bam.bai](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/?scope=project&id.values=file-GjQGjqj4qv8qyZ97xj57vjVq)|not versioned|
||`simrep`|[simpleRepeats_sorted_withoutchr.bed.gz](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/?scope=project&id.values=file-GjBQ30Q4qv8bQG728fZ81FbF)|not versioned|
||`simrep_index`|[simpleRepeats_sorted_withoutchr.bed.gz.tbi](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/?scope=project&id.values=file-GjBQ30Q4qv8kykJV7xxxf7z6)|not versioned|
||`genes`|[coding_unrestricted_GRCh38_myeloid_v1.2.bed](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/?scope=project&id.values=file-GjBQ30Q4qv8xv4PB054qYFfX) |v1.2|
||`unmatched`|[normalPanel_withoutchr.gff3.gz](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/?scope=project&id.values=file-GjBQb084qv8jGpk4GvJQPZx0)|not versioned|
||`filter`|[targetedRules.lst](https://platform.dnanexus.com/panx/projects/G21BGP84q5JFYf168QjZ58Vz/data/?scope=project&id.values=file-Fz8xvQj41zgGg10ZJzx8Qz53)|not versioned|
||`docker_image`|[cgppindel_image.tar.gz](https://platform.dnanexus.com/panx/projects/G21BGP84q5JFYf168QjZ58Vz/data/?scope=project&id.values=file-Fz0KxFj4KB7fxxZ06vy2B2P3)|not versioned|
|[verifybamid](https://github.com/eastgenomics/eggd_verifybamid)|`vcf_file`|[Omni25_genotypes_1525_samples_v2.b38.PASS.ALL.sites_no_chr.vcf.gz](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/?scope=project&id.values=file-G7YKFZj4kj47GxgQ2bKGYV1g)|not versioned|
|[picardqc](https://github.com/eastgenomics/eggd_picardqc)|`bedfile`|[Probes_GRCh38_HaemOnc_v2.1.bed](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/?scope=project&id.values=file-Ggv2k384jVYB0JX1Gjp669Bz)|v2.1|
|[mosdepth](https://github.com/eastgenomics/eggd_mosdepth)|`mosdepth_docker`|[mosdepth_image_v0.3.5.tar.gz](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/?scope=project&id.values=file-GbJXzq04pgpY6FX22Qvk9F9x)|v0.3.5||
|[athena](https://github.com/eastgenomics/athena)|`snps`|[hgmd_pro_2020.1_hg38.vcf](https://platform.dnanexus.com/panx/projects/G21BGP84q5JFYf168QjZ58Vz/data/?scope=project&id.values=file-FyZfyqQ41zg5FjK2GykYfKq8)| version 2020.1|
||`exons_file`|[exons_cellbase_GRCh38_5bp_flank_v2.1.0.tsv](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/?scope=project&id.values=file-GjBYbb04qv8VK56JYV335xk2)| v2.1.0|
||`panel_bed`|[coding_unrestricted_athena_GRCh38_myeloid_5bp_flank_v2.1.0.bed](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/?scope=project&id.values=file-GjBYbJ04qv8jp7Q0zQ4PX0f4)| v2.1.0|
|[somalier_extract](https://github.com/eastgenomics/eggd_somalier_extract)|`snp_site_vcf`|[sites.hg38.nochr.vcf](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/?scope=project&id.values=file-G7FJjz04kj424vq826gKbZx7)|not versioned|
||`somalier_docker`|[somalier_v0.2.16.tar.gz](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/assets/somalier)|v0.2.16|
||`reference_genome (sentieon)`|[GRCh38_GIABv3_no_alt_analysis_set_maskedGRC_decoys_MAP2K3_KMT2C_KCNJ18_noChr.fasta.gz](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/?scope=project&id.values=file-Gb757784XGyY3FPvkPQ74K9z)|not versioned|
||`reference_genome (other apps)`|[GRCh38_GIABv3_no_alt_analysis_set_maskedGRC_decoys_MAP2K3_KMT2C_KCNJ18_noChr.fa.gz](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/?scope=project&id.values=file-GjPxXq84qv8xz3ZV1jFq6z3g)|not versioned|
|[sompy](https://github.com/eastgenomics/eggd_sompy)|`truth_vcf`|[Horizon_44799.HD827.hg38.high_confident_NGS_and_ddPCR_variants_withoutchr.vcf.gz](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/?scope=project&id.values=file-Gjk675j4qv8zvQ5Qxq31Vfpg)|not versioned|
||`panel_bed`|[coding_unrestricted_GRCh38_myeloid_5bp_flank_v2.1.0.bed](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/?scope=project&id.values=file-Gj6YQg84qv8fkGzygZ19j300)|v2.1.0|
||`truth_high_`<br>`confidence_bed`|[HD827_variant_annotation_withoutchr.bed](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/?scope=project&id.values=file-Gj7BZj04qv8gx99jFB5QqV2y)|not versioned|
||`pkrusche_`<br>`happy_docker`|[pkrusche_happy_v0.3.9.tar.gz](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/?scope=project&id.values=file-GFGbK48433GzV4y54b25p43Z)|v0.3.9|
|[eggd_vep [mutect2 VCF]](https://github.com/eastgenomics/eggd_vep)|`config_file`|[uranus_vep_config_v1.2.1.json](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/dynamic_files/vep_configs)|v1.2.1|
||`panel_bed`|[coding_unrestricted_athena_GRCh38_myeloid_5bp_flank_v2.2.0.bed](https://platform.dnanexus.com/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/bed_files/b38/kits/myeloid?id.values=file-Gqy3qk847xBjBk1G7YV6YJ9V)|v2.2.0|
|[eggd_vep [cgppindel VCF]](https://github.com/eastgenomics/eggd_vep)|`config_file`|[uranus_vep_config_v1.2.1.json]([https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/dynamic_files/vep_configs?id.constraint=%24or&id.values=file-GyqQVVQ4B5QK34KF8180yj0P](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/dynamic_files/vep_configs))|v1.2.1|
||`panel_bed`|[pindel_cgppindel_filtering_coordinates_v1.2.bed](https://platform.dnanexus.com/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/bed_files/b38/kits/myeloid?id.values=file-Gqy4V1Q47xBXYzfKxb22fGXz)|v1.2|
|[eggd_vcf_rescue](https://github.com/eastgenomics/eggd_vcf_rescue)|`rescue_vcf`|[CosmicCodingMuts_GRCh38_v99.normal.NoEntry.vcf.gz](https://platform.dnanexus.com/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/?id.values=file-GjFv9X0421zQFGxXVFQ4j972)|v99|
||`fasta_tar`|[GRCh38_GIABv3_no_alt_analysis_set_maskedGRC_decoys_MAP2K3_KMT2C_KCNJ18_noChr.fasta-index.tar.gz](https://platform.dnanexus.com/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/?id.values=file-Gb772VQ4XGyzQ0Zk615XbZ0X)| not versioned |

---

### [multi_fastqc](https://github.com/eastgenomics/eggd_fastqc)

No external inputs.

---
### [somalier workflow](https://github.com/eastgenomics/eggd_somalier_workflow)

| App | Input field | Input file | Version |
|---  | ---   |---     | ---     |
| [somalier_relate](https://github.com/eastgenomics/eggd_somalier_relate) | `somalier_docker` | [somalier_v0.2.16.tar.gz](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/?name=somalier_v0.2.16.tar.gz&scope=project) | v0.2.16 |


---
### [MultiQC](https://github.com/eastgenomics/eggd_multiqc)

| Input field | Input file | Version |
| ---         | ---        | ---     |
| `multiqc_docker` | [seglh_multiqc_v1.11.tar.gz](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/?id.constraint=%24or&id.values=file-GF3PxgQ433Gqv1Q029Gjzjfv&scope=project) | v1.11.0 |
| `multiqc_config_file` | [MYE_multiqc_config_v2.1.0.yaml](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/?id.constraint=%24or&id.values=file-GF3Py30433GvZGb99kBVjZk1&scope=project) | v2.1.0 |
