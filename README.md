THIS REPOSITORY CONTAINS SCRIPTS AND DATA USED FOR MOTIF ENRICHMENT ANALYSIS EXPERIMENTALLY IDENTIFIED ENHANCERS BY STARR-SEQ

OVERVIEW OF FOLDERS: 

scripts/: 
    R-SCRIPTS AND BASH-SCRIPTS USED FOR THE ANALYSIS 
   
motifDB/: 
    PSCM-MATRICES FROM THE JASPAR VERTEBRATES CORE COLLECTION AND JASPAR CORE MATRIX CLUSTERING;
    ADDITIONALLY A TABLE WITH AN OVERVIEW OF SINGLE-TF MOTIFS ASSOCIATED WITH THE MOTIF CLUSTERS
    
STARRSseq_enhancer/: 
    BED-FILE WITH GENOMIC REGIONS OF ACTIVE mESC ENHANCERS OBTAINED BY STARRseq, FILTERED FOR PROMOTERS AND WIDTH-UNIFIED;
    ADDITIONALLY FASTA-FILES WITH GENOMIC SEQUENCES OF WEAK AND STRONG mESC AND RARa ENHANCERS
    
RESULTS_motifcounter/: 
    TABLES WITH RESULTS OF MOTIF ENRICHMENT ANALYSIS BY MOTIFCOUNTER ON WEAK AND STRONG mESC AND RARa ENHANCERS WITH SINGLE AND CLUSTERED MOTIFS;
    IN EACH TABLE MOTIFS ARE ORDERED IN DESCENDING ORDER BY THEIR ENRICHMENT;
    ADDITIONALLY DETAILED MOTIFCOUNTER RESULTS FOR mESC ENHANCERS WITH CLUSTERED MOTIFS IN TXT- AND RDS-FILE TO USE FOR CLASSIFIER LATER ON 
        
RESULTS_TRAP/: 
    TABLES WITH RESULTS OF MOTIF ENRICHMENT ANALYSIS BY TRAP ON WEAK AND STRONG mESC AND RARa ENHANCERS WITH SINGLE AND CLUSTERED MOTIFS;
    IN EACH TABLE MOTIFS ARE ORDERED IN DESCENDING ORDER BY THEIR ENRICHMENT (IN ASCENDING ORDER BY P-VALUE)
    
classifier/: 
    RDS-FILES WITH TEST- AND TRAINING-SETS AND GLMNET-OBJECT TO REPRODUCE RESUTLS IF NEEDED;
    ADDITIONALLY TABLE WITH BETA-COEFFICIENTS OF THE TRAINED REGRESSION MODEL