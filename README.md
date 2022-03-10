# utl-renaming-twenty-eight-variables-without-creating-a-new-dataset
Renaming twenty eight variables without creating a new dataset
    %let pgm=utl-renaming-twenty-eight-variables-without-creating-a-new-dataset;

    Renaming twenty eight variables without creating a new dataset

    SAS Communities
    https://tinyurl.com/43pu4b57
    https://communities.sas.com/t5/SAS-Enterprise-Guide/How-to-rename-variables-to-x1-x28-using-an-array/m-p/800752

    related repos
    https://tinyurl.com/yw8pttr9
    https://github.com/rogerjdeangelis?tab=repositories&q=renam&type=&language=&sort=

    /*
     _                   _
    (_)_ __  _ __  _   _| |_
    | | `_ \| `_ \| | | | __|
    | | | | | |_) | |_| | |_
    |_|_| |_| .__/ \__,_|\__|
            |_|
    */

    data have;
      retain
          pre_CHF
          pre_VALVE
          pre_PULMCIRC
          pre_PERIVASC
          pre_PARA
          pre_NEURO
          pre_CHRNLUNG
          pre_DM pre_DMCX
          pre_HTN_C
          pre_HYPOTHY
          pre_RENLFAIL
          pre_LIVER
          pre_ULCER
          pre_AIDS
          pre_LYMPH
          pre_METS
          pre_TUMOR
          pre_ARTH
          pre_COAG
          pre_OBESE
          pre_WGHTLOSS
          pre_BLDLOSS
          pre_ANEMDEF
          pre_ALCOHOL
          pre_DRUG
          pre_PSYCH
          pre_DEPRESS 0;
    run;quit;

    /**************************************************************************************************************************/
    /*                                                                                                                        */
    /* Up to 40 obs WORK.HAVE total obs=1 10MAR2022:11:21:47                                                                  */
    /*                                                                                                                        */
    /*   -- NUMERIC --                                                                                                        */
    /*                                                                                                                        */
    /*  Variable    TypeLength  Value                                                                                         */
    /*                                                                                                                        */
    /*  PRE_CHF          N8       0                                                                                           */
    /*  PRE_VALVE        N8       0                                                                                           */
    /*  PRE_PULMCIRC     N8       0                                                                                           */
    /*  PRE_PERIVASC     N8       0                                                                                           */
    /*  PRE_PARA         N8       0                                                                                           */
    /*  PRE_NEURO        N8       0                                                                                           */
    /*  PRE_CHRNLUNG     N8       0                                                                                           */
    /*  PRE_DM           N8       0                                                                                           */
    /*  PRE_DMCX         N8       0                                                                                           */
    /*  PRE_HTN_C        N8       0                                                                                           */
    /*  PRE_HYPOTHY      N8       0                                                                                           */
    /*  PRE_RENLFAIL     N8       0                                                                                           */
    /*  PRE_LIVER        N8       0                                                                                           */
    /*  PRE_ULCER        N8       0                                                                                           */
    /*  PRE_AIDS         N8       0                                                                                           */
    /*  PRE_LYMPH        N8       0                                                                                           */
    /*  PRE_METS         N8       0                                                                                           */
    /*  PRE_TUMOR        N8       0                                                                                           */
    /*  PRE_ARTH         N8       0                                                                                           */
    /*  PRE_COAG         N8       0                                                                                           */
    /*  PRE_OBESE        N8       0                                                                                           */
    /*  PRE_WGHTLOSS     N8       0                                                                                           */
    /*  PRE_BLDLOSS      N8       0                                                                                           */
    /*  PRE_ANEMDEF      N8       0                                                                                           */
    /*  PRE_ALCOHOL      N8       0                                                                                           */
    /*  PRE_DRUG         N8       0                                                                                           */
    /*  PRE_PSYCH        N8       0                                                                                           */
    /*  PRE_DEPRESS      N8       0                                                                                           */
    /*                                                                                                                        */
    /*                                                                                                                        */
    /**************************************************************************************************************************/

    /*           _               _
      ___  _   _| |_ _ __  _   _| |_
     / _ \| | | | __| `_ \| | | | __|
    | (_) | |_| | |_| |_) | |_| | |_
     \___/ \__,_|\__| .__/ \__,_|\__|
                    |_|
    */

    /**************************************************************************************************************************/
    /*                                                                                                                        */
    /* Up to 40 obs from HAVE total obs=1 10MAR2022:11:27:29                                                                  */
    /*                                                                                                                        */
    /*   -- NUMERIC --                                                                                                        */
    /*                                                                                                                        */
    /* Variable Type/Length  Value                                                                                            */
    /*                                                                                                                        */
    /*  X1       N8            0                                                                                              */
    /*  X2       N8            0                                                                                              */
    /*  X3       N8            0                                                                                              */
    /*  X4       N8            0                                                                                              */
    /*  X5       N8            0                                                                                              */
    /*  X6       N8            0                                                                                              */
    /*  X7       N8            0                                                                                              */
    /*  X8       N8            0                                                                                              */
    /*  X9       N8            0                                                                                              */
    /*  X10      N8            0                                                                                              */
    /*  X11      N8            0                                                                                              */
    /*  X12      N8            0                                                                                              */
    /*  X13      N8            0                                                                                              */
    /*  X14      N8            0                                                                                              */
    /*  X15      N8            0                                                                                              */
    /*  X16      N8            0                                                                                              */
    /*  X17      N8            0                                                                                              */
    /*  X18      N8            0                                                                                              */
    /*  X19      N8            0                                                                                              */
    /*  X20      N8            0                                                                                              */
    /*  X21      N8            0                                                                                              */
    /*  X22      N8            0                                                                                              */
    /*  X23      N8            0                                                                                              */
    /*  X24      N8            0                                                                                              */
    /*  X25      N8            0                                                                                              */
    /*  X26      N8            0                                                                                              */
    /*  X27      N8            0                                                                                              */
    /*  X28      N8            0                                                                                              */
    /*                                                                                                                        */
    /**************************************************************************************************************************/

    /*
     _ __  _ __ ___   ___ ___  ___ ___
    | `_ \| `__/ _ \ / __/ _ \/ __/ __|
    | |_) | | | (_) | (_|  __/\__ \__ \
    | .__/|_|  \___/ \___\___||___/___/
    |_|
    */

    * array of old names;
    %array(_oldnam,values=%varlist(have,keep=pre_:));

    /* macro variable _oldnamn = 28  */;

    * array of new names;
    %array(_newnam,values=1-&_oldnamn);

    *rename;
    proc datasets lib=work nodetails nolist;
      modify have;
      rename
          %do_over(_oldnam _newnam,phrase=%str(?_oldnam = x?_newnam));
    run;quit;

    * delete macro arrays;
    %arraydelete(_oldnam);
    %arraydelete(_newnam);

    %put &=_newnam28;

    /*
    | | ___   __ _
    | |/ _ \ / _` |
    | | (_) | (_| |
    |_|\___/ \__, |
             |___/
    */

    NOTE: Renaming variable PRE_CHF to X1.
    NOTE: Renaming variable PRE_VALVE to X2.
    NOTE: Renaming variable PRE_PULMCIRC to X3.
    NOTE: Renaming variable PRE_PERIVASC to X4.
    NOTE: Renaming variable PRE_PARA to X5.
    NOTE: Renaming variable PRE_NEURO to X6.
    NOTE: Renaming variable PRE_CHRNLUNG to X7.
    NOTE: Renaming variable PRE_DM to X8.
    NOTE: Renaming variable PRE_DMCX to X9.
    NOTE: Renaming variable PRE_HTN_C to X10.
    NOTE: Renaming variable PRE_HYPOTHY to X11.
    NOTE: Renaming variable PRE_RENLFAIL to X12.
    NOTE: Renaming variable PRE_LIVER to X13.
    NOTE: Renaming variable PRE_ULCER to X14.
    NOTE: Renaming variable PRE_AIDS to X15.
    NOTE: Renaming variable PRE_LYMPH to X16.
    NOTE: Renaming variable PRE_METS to X17.
    NOTE: Renaming variable PRE_TUMOR to X18.
    NOTE: Renaming variable PRE_ARTH to X19.
    NOTE: Renaming variable PRE_COAG to X20.
    NOTE: Renaming variable PRE_OBESE to X21.
    NOTE: Renaming variable PRE_WGHTLOSS to X22.
    NOTE: Renaming variable PRE_BLDLOSS to X23.
    NOTE: Renaming variable PRE_ANEMDEF to X24.
    NOTE: Renaming variable PRE_ALCOHOL to X25.
    NOTE: Renaming variable PRE_DRUG to X26.
    NOTE: Renaming variable PRE_PSYCH to X27.
    NOTE: Renaming variable PRE_DEPRESS to X28.
