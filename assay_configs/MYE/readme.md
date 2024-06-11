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
|[eggd_vcf_handler<br>_for_uranus](https://github.com/eastgenomics/eggd_vcf_handler_for_uranus)|`mutect2_bed`|[coding_unrestricted_GRCh38_myeloid_5bp_flank_v2.1.0.bed](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/?scope=project&id.values=file-Gj6YQg84qv8fkGzygZ19j300)|v2.1.0|
||`pindel_bed`|[pindel_cgppindel_filtering_coordinates_v1.1.bed](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/?scope=project&id.values=file-Gj6YXj84qv8YV5Z3yb2Zk6Pg)|v1.1|
||`vep_annotation`|[clinvar_20240514_GRCh38.vcf.gz](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/annotation/b38/clinvar)|version 20240514|
||`vep_annotation`|[clinvar_20240514_GRCh38.vcf.gz.tbi](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/annotation/b38/clinvar)|version 20240514|
||`vep_refs`|[gnomad.genomes.r3.0.indel.tsv.gz](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/?scope=project&id.values=file-G61xbP0433GqX36p8QQxP3PV)|version r3.0|
||`vep_refs`|[gnomad.genomes.r3.0.indel.tsv.gz.tbi](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/?scope=project&id.values=file-G61xf3j433Gz49jf6XjKG4F0)|version r3.0|
||`vep_refs`|[whole_genome_SNVs.tsv.gz](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/?scope=project&id.values=file-G61xfZ0433Gj2vJ7P8k9ky2Z)| not versioned|
||`vep_refs`|[whole_genome_SNVs.tsv.gz.tbi](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/?scope=project&id.values=file-G61y4Y8433GvyjJ52Fj5XjY5)|not versioned|
||`vep_annotation`|[CosmicCodingMuts_GRCh38_v99.normal.vcf.gz](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/?scope=project&id.values=file-Gf02Fxj4Pj2vPPV0zyfpbFkz)|v99|
||`vep_annotation`|[CosmicCodingMuts_GRCh38_v99.normal.vcf.gz.tbi](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/?scope=project&id.values=file-Gf02JgQ4Pj2xZg2b1g9pVV7g)|v99|
||`vep_annotation`|[CosmicNonCodingVariants_GRCh38_v99.normal.vcf.gz](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/?scope=project&id.values=file-Gf02Jj04Pj2ZPxF97V6YJFKv)|v99|
||`vep_annotation`|[CosmicNonCodingVariants_GRCh38_v99.normal.vcf.gz.tbi](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/?scope=project&id.values=file-Gf02KG84Pj2QB86kK721B9yQ)|v99|
||`vep_docker`|[vep_v103.1_docker.tar.gz](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/?scope=project&id.values=file-G61zff8433Gy2KQX7Q2z150B)|v103.1|
||`vep_plugins`|[plugin_config.txt](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/?scope=project&id.values=file-G61zfvj433GxkQXF414xP1yF)| not versioned|
||`vep_plugins`|[ CADD.pm](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/?scope=project&id.values=file-G620928433Gy9p2b27zb8JFV)|not versioned|
||`vep_refs`|[Homo_sapiens.GRCh38.dna.toplevel.fa.gz](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/?scope=project&id.values=file-G61y95Q433Gk05zyFKF9kFv2)|not versioned|
||`vep_refs`|[Homo_sapiens.GRCh38.dna.toplevel.fa.gz.fai](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/?scope=project&id.values=file-G61yBV8433GjbVj022PyV3K5)|not versioned|
||`vep_refs`|[Homo_sapiens.GRCh38.dna.toplevel.fa.gz.gzi](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/?scope=project&id.values=file-G61yBf0433Gp4BBVGj0jxqvP)|not versioned|
||`vep_refs`|[homo_sapiens_refseq_vep_103_GRCh38.tar.gz](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/?scope=project&id.values=file-G61yF38433GQgP504Px5PZ4G)|not versioned|
||`maf_file`|[haemonc_1706_samples_withoutchr.vcf.gz](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/?scope=project&id.values=file-Gj6YQg84qv8v2J1XKJy4fQYg)|not versioned|
||`maf_file_tbi`|[haemonc_1706_samples_withoutchr.vcf.gz.tbi](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/?scope=project&id.values=file-Gj6YQg84qv8Z3F4J8fX7YK6V)|not versioned|

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
