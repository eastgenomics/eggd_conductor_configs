## 📄 Uranus input files

Below defines all external input files, their versions and file locations in DNAnexus used as part of the Uranus pipeline. These are used in the eggd_conductor assay config file within the `inputs` section for each executable

---
### [Uranus main workflow](https://github.com/eastgenomics/eggd_uranus_main_workflow)

| App 	| Input field |  Input file 	| Version  	|
|---	|---	|---	|--- |
|[cgppindel](https://github.com/eastgenomics/eggd_cgppindel)| `normal` |[TA2_S59_L008_tumor_markdup.bam](https://platform.dnanexus.com/panx/projects/G21BGP84q5JFYf168QjZ58Vz/data/?scope=project&id.values=file-Fy9BXxQ40vjGfxP46Jb78Xf1)|not versioned|
||`normal_index`|[TA2_S59_L008_tumor_markdup.bam.bai](https://platform.dnanexus.com/panx/projects/G21BGP84q5JFYf168QjZ58Vz/data/?scope=project&id.values=file-Fy9BXxQ40vj7qPJq1Kppjx0F)|not versioned|
||`simrep`|[simpleRepeats_sorted.bed.gz](https://platform.dnanexus.com/panx/projects/G21BGP84q5JFYf168QjZ58Vz/data/?scope=project&id.values=file-Fz0Q2GQ41zgB8BK7143y65Q1)|not versioned|
||`simrep_index`|[simpleRepeats_sorted.bed.gz.tbi](https://platform.dnanexus.com/panx/projects/G21BGP84q5JFYf168QjZ58Vz/data/?scope=project&id.values=file-Fz0Q2Kj41zg0Fgk4G70P9P1X)|not versioned|
||`genes`|[coding_unrestricted_GRCh38_myeloid_v1.0.bed](https://platform.dnanexus.com/panx/projects/G21BGP84q5JFYf168QjZ58Vz/data/?scope=project&id.values=file-FybyxV841zgB8v1y3fFbFB0G) |v1.0|
||`unmatched`|[normalPanel.gff3.gz](https://platform.dnanexus.com/panx/projects/G21BGP84q5JFYf168QjZ58Vz/data/?scope=project&id.values=file-Fz8Q0vj41zg6j03fP1vbvfFp)|not versioned|
||`filter`|[targetedRules.lst](https://platform.dnanexus.com/panx/projects/G21BGP84q5JFYf168QjZ58Vz/data/?scope=project&id.values=file-Fz8xvQj41zgGg10ZJzx8Qz53)|not versioned|
||`docker_image`|[cgppindel_image.tar.gz](https://platform.dnanexus.com/panx/projects/G21BGP84q5JFYf168QjZ58Vz/data/?scope=project&id.values=file-Fz0KxFj4KB7fxxZ06vy2B2P3)|not versioned|
|[verifybamid](https://github.com/eastgenomics/eggd_verifybamid)|`vcf_file`|[Omni25_genotypes_1525_samples_v2.b38.PASS.ALL.sites.vcf.gz](https://platform.dnanexus.com/panx/projects/G21BGP84q5JFYf168QjZ58Vz/data/?scope=project&id.values=file-G07zJxj41zgF593x6j7bqZ7X)|not versioned|
|[picardqc](https://github.com/eastgenomics/eggd_picardqc)|`bedfile`|[Probes_GRCh38_HaemOnc_v2.0.bed](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/?scope=project&id.values=file-G9vKbv0433GjJv1j7gp0P9vx)|v2.0|
|[athena](https://github.com/eastgenomics/athena)|`snps`|[hgmd_pro_2020.1_hg38.vcf](https://platform.dnanexus.com/panx/projects/G21BGP84q5JFYf168QjZ58Vz/data/?scope=project&id.values=file-FyZfyqQ41zg5FjK2GykYfKq8)| version 2020.1|
||`exons_file`|[exons_cellbase_GRCh38_5bp_flank_v2.0.0.tsv](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/?scope=project&id.values=file-G9vKbv0433GVJQ4BK701FjBB)| v2.0.0|
||`panel_bed`|[coding_unrestricted_athena_GRCh38_myeloid_5bp_flank_v2.0.0.bed](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/?scope=project&id.values=file-G9vKbv0433GxkgqK2GJj79fP)| v2.0.0|
|[somalier_extract](https://github.com/eastgenomics/eggd_somalier_extract)|`snp_site_vcf`|[sites.hg38.vcf](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/?scope=project&id.values=file-G9vXxp8433Gz8jz02fbyKzVj)|not versioned|
|[sompy](https://github.com/eastgenomics/eggd_sompy)|`truth_vcf`|[Horizon_44799.HD827.hg38.high_confident_NGS_and_ddPCR_variants.vcf.gz](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/?scope=project&id.values=file-GF3BJJj433Gzgy6qJGx52Gjg)|not versioned|
||`panel_bed`|[coding_unrestricted_GRCh38_myeloid_5bp_flank_v2.0.0.bed](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/?scope=project&id.values=file-G9vKbv0433Gg2bP9GP72pxKJ)|v2.0.0|
||`truth_high_`<br>`confidence_bed`|[HD827_variant_annotation.bed](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/?scope=project&id.values=file-GF3BJ1j433GZgy5x486Xyk5B)|not versioned|
||`pkrusche_`<br>`happy_docker`|[pkrusche_happy_v0.3.9.tar.gz](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/?scope=project&id.values=file-GFGbK48433GzV4y54b25p43Z)|v0.3.9|
|[eggd_vcf_handler<br>_for_uranus](https://github.com/eastgenomics/eggd_vcf_handler_for_uranus)|`mutect2_bed`|[coding_unrestricted_GRCh38_myeloid_5bp_flank_v2.0.0.bed](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/?scope=project&id.values=file-G9vKbv0433Gg2bP9GP72pxKJ)|v2.0.0|
||`pindel_bed`|[pindel_cgppindel_filtering_coordinates_v1.0.bed](https://platform.dnanexus.com/panx/projects/G21BGP84q5JFYf168QjZ58Vz/data/?scope=project&id.values=file-G0bFvXQ433GZJq780QgxZxKf)|v1.0|
||`vep_annotation`|[clinvar_20230218_b38_withchr.vcf.gz](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/annotation/b38/clinvar)|version 20230218|
||`vep_annotation`|[clinvar_20230218_b38_withchr.vcf.gz.tbi](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/annotation/b38/clinvar)|version 20230218|
||`vep_refs`|[gnomad.genomes.r3.0.indel.tsv.gz](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/?scope=project&id.values=file-G61xbP0433GqX36p8QQxP3PV)|version r3.0|
||`vep_refs`|[gnomad.genomes.r3.0.indel.tsv.gz.tbi](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/?scope=project&id.values=file-G61xf3j433Gz49jf6XjKG4F0)|version r3.0|
||`vep_refs`|[whole_genome_SNVs.tsv.gz](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/?scope=project&id.values=file-G61xfZ0433Gj2vJ7P8k9ky2Z)| not versioned|
||`vep_refs`|[whole_genome_SNVs.tsv.gz.tbi](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/?scope=project&id.values=file-G61y4Y8433GvyjJ52Fj5XjY5)|not versioned|
||`vep_annotation`|[CosmicCodingMuts_GRCh38_v94.normal.vcf.gz](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/?scope=project&id.values=file-G64Jfk0433GVp0JJPZ4Q8FzJ)|v94|
||`vep_annotation`|[CosmicCodingMuts_GRCh38_v94.normal.vcf.gz.tbi](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/?scope=project&id.values=file-G64K4bj433GZ35xJJ7YXGvzv)|v94|
||`vep_annotation`|[CosmicNonCodingVariants_GRCh38_v94.normal.vcf.gz](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/?scope=project&id.values=file-G64K0VQ433GV03462J6GXb9Z)|v94|
||`vep_annotation`|[CosmicNonCodingVariants_GRCh38_v94.normal.vcf.gz.tbi](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/?scope=project&id.values=file-G64K4j8433Gb0PgpFgbzjj1b)|v94|
||`vep_docker`|[vep_v103.1_docker.tar.gz](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/?scope=project&id.values=file-G61zff8433Gy2KQX7Q2z150B)|v103.1|
||`vep_plugins`|[plugin_config.txt](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/?scope=project&id.values=file-G61zfvj433GxkQXF414xP1yF)| not versioned|
||`vep_plugins`|[ CADD.pm](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/?scope=project&id.values=file-G620928433Gy9p2b27zb8JFV)|not versioned|
||`vep_refs`|[Homo_sapiens.GRCh38.dna.toplevel.fa.gz](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/?scope=project&id.values=file-G61y95Q433Gk05zyFKF9kFv2)|not versioned|
||`vep_refs`|[Homo_sapiens.GRCh38.dna.toplevel.fa.gz.fai](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/?scope=project&id.values=file-G61yBV8433GjbVj022PyV3K5)|not versioned|
||`vep_refs`|[Homo_sapiens.GRCh38.dna.toplevel.fa.gz.gzi](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/?scope=project&id.values=file-G61yBf0433Gp4BBVGj0jxqvP)|not versioned|
||`vep_refs`|[homo_sapiens_refseq_vep_103_GRCh38.tar.gz](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/?scope=project&id.values=file-G61yF38433GQgP504Px5PZ4G)|not versioned|
||`maf_file`|[novaseq_205samples_211007.vcf.gz](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/?scope=project&id.values=file-G5PXK90433GjKFq70yfz9qfZ)| version 211007|
||`maf_file_tbi`|[novaseq_205samples_211007.vcf.gz.tbi](https://platform.dnanexus.com/panx/projects/Fkb6Gkj433GVVvj73J7x8KbV/data/?scope=project&id.values=file-G5PXKFj433Gv495095Z95pk1)| version 211007|

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
