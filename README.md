snakemake -s atacseq_pipeline.snake --use-conda dryrun

snakemake -s atacseq_pipeline.snake --use-conda --cores 16 --jobs 16 --cluster "qsub -cwd -P langchip -pe smp 16"
