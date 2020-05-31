# Proyecto_Bioinf2020

Para estimar la divergencia entre poblaciones e inferir procesos evolutivos se obtuvimos una representación reducida del genoma usando el Genotipo basado en secuencia (SBG) para el descubrimiento del Polimorfismo de nucleótido único (SNP).
El Centro de Genómica de la Universidad de Minnesota (UMGC) realizó la construcción de la biblioteca, la secuenciación, el filtrado de calidad primaria, el tratamiento informático y las llamadas SNP.

Se recivio un archivo ``vcf`` con **109299 SNPs** que se obtuvo a partir de prepararon 93 bibliotecas de doble índice a partir de ADN doblemente digerido con enzimas MSPI y NsiI-HF, siguiendo el protocolo estándar UMGC para la preparación de la biblioteca SBG y códigos de barras individuales (Truong et al., 2012). Las bibliotecas se combinaron en un solo grupo y se secuenciaron en una ejecución Illumina®️ NextSeq 550 1x150-bp. 

A partir del archivo con **109299 SNPs** se realizó un filtrado de variantes con ayuda del software ``VCFtools.v.0.1.15`` dentro de un repositorio de docker `biocontainers/vcftools:0.1.15`, se aplicaron filtros para conservar solo variantes sin llamadas perdidas y eliminamos sitios no informativos (MAF <0.05) el script se encuentra dentro de la carpeta **bin**: [VCFtools_copepodos.sh](https://github.com/JavierUrban/Proyecto_Bioinf2020/blob/master/bin/VCFtools_copepodos.sh) 

Después de los filtros aplicados con ``VCFtools`` se recupero un total de **11254 SNPs** que se usaron para analizar y describir la estructura genética con  ``R software``, se detalla los pasos en el script: [Gen_Pop_Copes.R](https://github.com/JavierUrban/Proyecto_Bioinf2020/blob/master/bin/Gen_PoP_Copes.R) dentro de la carpeta bin 

Una explicación general de la divergencia genética de las poblaciones de los copépodos *Leptodiaptomus* la puedes encontrar en: [Reporte_general.md](https://github.com/JavierUrban/Proyecto_Bioinf2020/blob/master/Reporte%20general.md) donde se encuentran algunas figuras de los resultados obtenidos. 

Los scripts se corren asumiendo que están en la carpeta [bin](https://github.com/JavierUrban/Proyecto_Bioinf2020/tree/master/bin), los datos archivos vcf y una tabla con los nombre de los individuos y las poblaciones en [data](https://github.com/JavierUrban/Proyecto_Bioinf2020/tree/master/data).
