# /*------------------------------------------------------------\
# |                                                             |
# | File   :                    Makefile                        |
# |                                                             |
# | Author :                 Jacomme Ludovic                    |
# |                                                             |
# \------------------------------------------------------------*/
# /*------------------------------------------------------------\
# |                                                             |
# |                              Cells                          |
# |                                                             |
# \------------------------------------------------------------*/
# /*------------------------------------------------------------\
# |                                                             |
# |                             Binary                          |
# |                                                             |
# \------------------------------------------------------------*/

#ALLIANCE_BIN=$(ALLIANCE_TOP)/usr/bin

#ALLIANCE_EXAMPLES=/home/abuahmedin/Documents/Alliance/alliance/examples/alliance-examples/
include ../etc/alliance-env.mk

VASY   = $(ALLIANCE_BIN)/vasy
ASIMUT = $(ALLIANCE_BIN)/asimut
BOOM   = $(ALLIANCE_BIN)/boom
BOOG   = $(ALLIANCE_BIN)/boog
LOON   = $(ALLIANCE_BIN)/loon
OCP    = $(ALLIANCE_BIN)/alliance-ocp
NERO   = $(ALLIANCE_BIN)/nero
RING   = $(ALLIANCE_BIN)/ring
COUGAR = $(ALLIANCE_BIN)/alliance-cougar
LVX    = $(ALLIANCE_BIN)/lvx
DRUC   = $(ALLIANCE_BIN)/druc
S2R    = $(ALLIANCE_BIN)/s2r

DREAL  = $(ALLIANCE_BIN)/dreal
GRAAL  = $(ALLIANCE_BIN)/graal
XSCH   = $(ALLIANCE_BIN)/xsch
XPAT   = $(ALLIANCE_BIN)/xpat
XFSM   = $(ALLIANCE_BIN)/xfsm

TOUCH  = touch

TARGET_LIB      = $(CELLS_TOP)/sxlib
#METAL_LEVEL     = 2



#TARGET_LIB	=$(ALLIANCE_TOP)/usr/share/alliance/cells/sxlib
#RDS_TECHNO_SYMB	=/etc/cmos.rds
#RDS_TECHNO	=/etc/cmos.rds
#SPI_MODEL	=/etc/spimodel.cfg
#MBK_CATA_LIB     =.:/usr/share/alliance/cells/sxlib:/usr/share/alliance/cells/rflib:/usr/share/alliance/cells/rf2lib:/usr/share/alliance/cells/romlib:/usr/share/#alliance/cells/pxlib:/usr/share/alliance/cells/padlib
METAL_LEVEL     = 4


# /*------------------------------------------------------------\
# |                                                             |
# |                            Environment                     |
# |                                                             |
# \------------------------------------------------------------*/

ENV_VASY = MBK_WORK_LIB=.; export MBK_WORK_LIB;\
           MBK_CATAL_NAME=NO_CATAL; export MBK_CATAL_NAME

ENV_BOOM = MBK_WORK_LIB=.; export MBK_WORK_LIB;\
           MBK_CATAL_NAME=CATAL; export MBK_CATAL_NAME

ENV_BOOG = MBK_WORK_LIB=.; export MBK_WORK_LIB; \
           MBK_IN_LO=vst; export MBK_IN_LO; \
	   MBK_OUT_LO=vst; export MBK_OUT_LO; \
           MBK_TARGET_LIB=$(TARGET_LIB); export MBK_TARGET_LIB; \
           MBK_CATAL_NAME=CATAL; export MBK_CATAL_NAME

ENV_LOON = MBK_WORK_LIB=.; export MBK_WORK_LIB; \
           MBK_IN_LO=vst; export MBK_IN_LO; \
	   MBK_OUT_LO=vst; export MBK_OUT_LO; \
           MBK_TARGET_LIB=$(TARGET_LIB); export MBK_TARGET_LIB; \
           MBK_CATA_LIB=$(MBK_CATA_LIB); export MBK_CATA_LIB; \
           MBK_CATAL_NAME=CATAL; export MBK_CATAL_NAME

ENV_ASIMUT_VASY = MBK_WORK_LIB=.; export MBK_WORK_LIB;\
             MBK_CATAL_NAME=CATAL_ASIMUT_VASY; export MBK_CATAL_NAME;\
             MBK_IN_LO=vst; export MBK_IN_LO;\
	     MBK_OUT_LO=vst; export MBK_OUT_LO

ENV_ASIMUT_SYNTH = MBK_WORK_LIB=.; export MBK_WORK_LIB;\
             MBK_CATAL_NAME=CATAL; export MBK_CATAL_NAME;\
             MBK_CATA_LIB=$(MBK_CATA_LIB); export MBK_CATA_LIB; \
             MBK_IN_LO=vst; export MBK_IN_LO;\
	     MBK_OUT_LO=vst; export MBK_OUT_LO

ENV_OCP =  MBK_WORK_LIB=.; export MBK_WORK_LIB; \
           MBK_IN_LO=vst; export MBK_IN_LO; \
	   MBK_OUT_LO=vst; export MBK_OUT_LO; \
           MBK_CATA_LIB=$(MBK_CATA_LIB); export MBK_CATA_LIB; \
           MBK_IN_PH=ap; export MBK_IN_PH; \
           MBK_OUT_PH=ap; export MBK_OUT_PH; \
           MBK_CATAL_NAME=CATAL; export MBK_CATAL_NAME

ENV_NERO =  MBK_WORK_LIB=.; export MBK_WORK_LIB; \
           MBK_IN_LO=vst; export MBK_IN_LO; \
	   MBK_OUT_LO=vst; export MBK_OUT_LO; \
           MBK_CATA_LIB=$(MBK_CATA_LIB); export MBK_CATA_LIB; \
           MBK_IN_PH=ap; export MBK_IN_PH; \
           MBK_OUT_PH=ap; export MBK_OUT_PH; \
           MBK_CATAL_NAME=CATAL; export MBK_CATAL_NAME



ENV_COUGAR_SPI =  MBK_WORK_LIB=.; export MBK_WORK_LIB; \
           MBK_IN_LO=spi; export MBK_IN_LO; \
	   MBK_OUT_LO=spi; export MBK_OUT_LO; \
           MBK_SPI_MODEL=$(SPI_MODEL); export MBK_SPI_MODEL; \
           MBK_SPI_ONE_NODE_NORC="true"; export MBK_SPI_ONE_NODE_NORC; \
           MBK_SPI_NAMEDNODES="true"; export MBK_SPI_NAMEDNODES; \
           RDS_TECHNO_NAME=$(RDS_TECHNO); export RDS_TECHNO_NAME; \
           RDS_IN=cif; export RDS_IN; \
           RDS_OUT=cif; export RDS_OUT; \
           MBK_CATA_LIB=$(MBK_CATA_LIB); export MBK_CATA_LIB; \
           MBK_IN_PH=ap; export MBK_IN_PH; \
           MBK_OUT_PH=ap; export MBK_OUT_PH; \
           MBK_CATAL_NAME=CATAL; export MBK_CATAL_NAME

ENV_COUGAR =  MBK_WORK_LIB=.; export MBK_WORK_LIB; \
           MBK_IN_LO=al; export MBK_IN_LO; \
	   MBK_OUT_LO=al; export MBK_OUT_LO; \
           RDS_TECHNO_NAME=$(RDS_TECHNO); export RDS_TECHNO_NAME; \
           RDS_IN=cif; export RDS_IN; \
           RDS_OUT=cif; export RDS_OUT; \
           MBK_CATA_LIB=$(MBK_CATA_LIB); export MBK_CATA_LIB; \
           MBK_IN_PH=ap; export MBK_IN_PH; \
           MBK_OUT_PH=ap; export MBK_OUT_PH; \
           MBK_CATAL_NAME=CATAL; export MBK_CATAL_NAME

ENV_LVX =  MBK_WORK_LIB=.; export MBK_WORK_LIB; \
           MBK_IN_LO=vst; export MBK_IN_LO; \
	   MBK_OUT_LO=vst; export MBK_OUT_LO; \
           MBK_CATA_LIB=$(MBK_CATA_LIB); export MBK_CATA_LIB; \
           MBK_CATAL_NAME=CATAL; export MBK_CATAL_NAME

ENV_DRUC = MBK_WORK_LIB=.; export MBK_WORK_LIB; \
           RDS_TECHNO_NAME=$(RDS_TECHNO_SYMB); export RDS_TECHNO_NAME; \
           MBK_IN_PH=ap; export MBK_IN_PH; \
           MBK_OUT_PH=ap; export MBK_OUT_PH; \
           MBK_CATA_LIB=$(MBK_CATA_LIB); export MBK_CATA_LIB; \
           MBK_CATAL_NAME=CATAL; export MBK_CATAL_NAME

ENV_S2R  = MBK_WORK_LIB=.; export MBK_WORK_LIB; \
           RDS_TECHNO_NAME=$(RDS_TECHNO); export RDS_TECHNO_NAME; \
           RDS_IN=cif; export RDS_IN; \
           RDS_OUT=cif; export RDS_OUT; \
           MBK_IN_PH=ap; export MBK_IN_PH; \
           MBK_OUT_PH=ap; export MBK_OUT_PH; \
           MBK_CATA_LIB=$(MBK_CATA_LIB); export MBK_CATA_LIB; \
           MBK_CATAL_NAME=CATAL; export MBK_CATAL_NAME

#  Alliance paths and formats settings.
 GENERAT_LO   = vst
 EXTRACT_LO   = al
 CARAC_LO     = spi
 GENERAT_PH   = ap
 EXTRACT_PH   = ap
 GENERAT_SP   = .
 EXTRACT_SP   = .

 ENV_RING =       MBK_TARGET_LIB=$(TARGET_LIB);  	export MBK_TARGET_LIB;\
                   MBK_WORK_LIB=.;                	export MBK_WORK_LIB;  \
                   MBK_CATA_LIB=$(MBK_CATA_LIB);      	export MBK_CATA_LIB;  \
                   MBK_CATAL_NAME=CATAL;          	export MBK_CATAL_NAME;\
                   MBK_OUT_LO=$(GENERAT_LO);      	export MBK_OUT_LO;    \
                   MBK_OUT_PH=$(GENERAT_PH);      	export MBK_OUT_PH;    \
                   MBK_IN_LO=$(GENERAT_LO);       	export MBK_IN_LO;     \
                   MBK_IN_PH=$(GENERAT_PH);       	export MBK_IN_PH;     \
                   MBK_SEPAR=$(GENERAT_SP);       	export MBK_SEPAR;     \
                   MBK_VDD=vdd;                 	export MBK_VDD;       \
                   MBK_VSS=vss;                   	export MBK_VSS;       \
		   RDS_TECHNO_NAME=$(RDS_TECHNO);	export RDS_TECHNO_NAME


all : filter.cif  

# /*------------------------------------------------------------\
# |                                                             |
# |                             Vasy                            |
# |                                                             |
# \------------------------------------------------------------*/

filter.vbe : filter.vhdl
	$(ENV_VASY); $(VASY) -a -B -o -p -I vhdl filter

# /*------------------------------------------------------------\
# |                                                             |
# |                             Asimut                          |
# |                                                             |
# \------------------------------------------------------------*/

res_vasy_1.pat : filter.vbe
	$(ENV_ASIMUT_VASY); $(ASIMUT) -b filter filter res_vasy_1 

res_synth_1.pat : filter.vst 
	$(ENV_ASIMUT_SYNTH); $(ASIMUT) filter filter res_synth_1

# /*------------------------------------------------------------\
# |                                                             |
# |                             Boom                            |
# |                                                             |
# \------------------------------------------------------------*/

boom.done : filter_o.vbe
	@$(TOUCH) boom.done

filter_o.vbe : filter.vbe filter.boom res_vasy_1.pat
	$(ENV_BOOM); $(BOOM) -VP filter filter_o

# /*------------------------------------------------------------\
# |                                                             |
# |                             Boog                            |
# |                                                             |
# \------------------------------------------------------------*/

boog.done : filter_o.vst
	@$(TOUCH) boog.done

filter_o.vst : filter_o.vbe
	$(ENV_BOOG); $(BOOG) filter_o

# /*------------------------------------------------------------\
# |                                                             |
# |                             Loon                            |
# |                                                             |
# \------------------------------------------------------------*/

loon.done : filter.vst
	@$(TOUCH) loon.done

filter.vst : filter_o.vst
	$(ENV_LOON); $(LOON) filter_o filter

# /*------------------------------------------------------------\
# |                                                             |
# |                             OCP                             |
# |                                                             |
# \------------------------------------------------------------*/

filter_p.ap : res_synth_1.pat
	$(ENV_OCP); $(OCP) -v -gnuplot -ioc filter  filter filter_p

# /*------------------------------------------------------------\
# |                                                             |
# |                             NERO                            |
# |                                                             |
# \------------------------------------------------------------*/

filter.ap : filter_p.ap filter.vst
	$(ENV_NERO); $(NERO) -V -$(METAL_LEVEL) -p filter_p filter filter

# /*------------------------------------------------------------\
# |                                                             |
# |                             Cougar                          |
# |                                                             |
# \------------------------------------------------------------*/

filter_e.spi : filter.ap
	$(ENV_COUGAR_SPI); $(COUGAR) -v -ac filter filter_e

filter_erc.spi : filter.ap
	$(ENV_COUGAR_SPI); $(COUGAR) -v -ar filter filter_erc

filter_erc.al : filter.ap
	$(ENV_COUGAR); $(COUGAR) -v -ar filter filter_erc

filter_e.al : filter.ap
	$(ENV_COUGAR); $(COUGAR) -v -ac filter filter_e

filter_et.al : filter.ap
	$(ENV_COUGAR); $(COUGAR) -v -ac -t filter filter_et

filter_et.spi : filter.ap
	$(ENV_COUGAR_SPI); $(COUGAR) -v -ac -t filter filter_et

filter_er.al : filter.cif
	$(ENV_COUGAR); $(COUGAR) -v -r -t filter filter_er

filter_real.al : filter.ap
	$(ENV_COUGAR); $(ENV_S2R); $(COUGAR) -v -ac filter filter_real

filter_real_t.al : filter.ap
	$(ENV_COUGAR); $(ENV_S2R); $(COUGAR) -v -t -ac filter filter

filter.al : filter.ap
	$(ENV_COUGAR); $(ENV_S2R); $(COUGAR) -c filter filter

# /*------------------------------------------------------------\
# |                                                             |
# |                             Lvx                             |
# |                                                             |
# \------------------------------------------------------------*/

lvx.done : filter.vst filter_e.al filter_e.spi
	$(ENV_LVX); $(LVX) vst al filter filter_e -f
	$(TOUCH) lvx.done

# /*------------------------------------------------------------\
# |                                                             |
# |                             Druc                            |
# |                                                             |
# \------------------------------------------------------------*/

druc.done : lvx.done filter.ap
	$(ENV_DRUC); $(DRUC) filter
	$(TOUCH) druc.done

# /*------------------------------------------------------------\
# |                                                             |
# |                             S2R                             |
# |                                                             |
# \------------------------------------------------------------*/

filter.cif : druc.done
	$(ENV_S2R); $(S2R) -v filter filter

# /*------------------------------------------------------------\
# |                                                             |
# |                             Ring                             |
# |                                                             |
# \------------------------------------------------------------*/


filter_pad.ap : filter_chip.vst  filter_chip.rin
	$(ENV_RING); $(RING)  filter_chip filter_pad 
    
# /*------------------------------------------------------------\
# |                                                             |
# |                             S2R                             |
# |                                                             |
# \------------------------------------------------------------*/

filter_pad.cif : filter_pad.ap
	$(ENV_S2R); $(S2R) -v filter_pad filter_pad
# /*------------------------------------------------------------\
# |                                                             |
# |                             TOOLS                           |
# |                                                             |
# \------------------------------------------------------------*/

graal :
	$(ENV_S2R); $(GRAAL)

graal_filter_p : filter_p.ap
	$(ENV_S2R); $(GRAAL) -l filter_p

graal_filter : filter.ap
	$(ENV_S2R); $(GRAAL) -l filter

xsch:
	$(ENV_LOON); $(XSCH)

xsch_filter_o : filter.vst
	$(ENV_LOON); $(XSCH) -l filter_o

xsch_filter : filter.vst
	$(ENV_LOON); $(XSCH) -l filter

xsch_filter_e: filter_e.al
	$(ENV_COUGAR); $(XSCH) -l filter_e

xsch_filter_et: filter_et.al
	$(ENV_COUGAR); $(XSCH) -l filter_et

xpat: 
	$(ENV_ASIMUT_SYNTH); $(XPAT)

xpat_synth: res_synth_1.pat
	$(ENV_ASIMUT_SYNTH); $(XPAT) -l res_synth_1

xpat_vasy : res_vasy_1.pat
	$(ENV_ASIMUT_SYNTH); $(XPAT) -l res_vasy_1

dreal: 
	$(ENV_S2R); $(DREAL)

dreal_filter : filter.cif
	$(ENV_S2R); $(DREAL) -l filter


# /*------------------------------------------------------------\
# |                                                             |
# |                              Clean                          |
# |                                                             |
# \------------------------------------------------------------*/

realclean : clean

clean     :
	$(RM) -f *.vst filter_e.spi filter_et.spi *.vbe res_*.pat *.boom *.done *.xsc *.gpl \
                 *.ap *.drc *.dat *.gds *.cif *.rep \
		 *.log *.out *.raw *.al
