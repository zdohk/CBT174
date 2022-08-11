~~~~~~~~~~~~~~~~

//***FILE 174 IS THE "TAPECOPY" PROGRAM FROM ARON EISENPRESS OF     *   FILE 174
//*           THE CITY UNIVERSITY COMPUTER CENTER IN NEW YORK.      *   FILE 174
//*           AMONG ITS MANY OPTIONS, IS THE ABILITY TO CREATE      *   FILE 174
//*           A STANDARD-LABELED TAPE FROM A NON-LABELED TAPE.      *   FILE 174
//*           (I USED THIS FEATURE AS PART OF MY PROCESSING OF      *   FILE 174
//*           THE CBT TAPE - EDITOR.)  MANY ADJUSTMENTS CAN BE      *   FILE 174
//*           MADE IN THE PROCESSING TO BE ABLE TO HANDLE           *   FILE 174
//*           MESSED-UP AND UNUSUAL TAPES.                          *   FILE 174
//*                                                                 *   FILE 174
//*           Aron Eisenpress                                       *   FILE 174
//*           Manager, MVS Systems                                  *   FILE 174
//*           City University of New York                           *   FILE 174
//*           Computing and Information Services                    *   FILE 174
//*           555 West 57th Street, 16th floor                      *   FILE 174
//*           New York, New York  10019-2919                        *   FILE 174
//*                                                                 *   FILE 174
//*           Phone: 212/541-0918                                   *   FILE 174
//*                                                                 *   FILE 174
//*           email: afecu@cunyvm.cuny.edu                          *   FILE 174
//*                                                                 *   FILE 174
//*      THIS IS A GENERALIZED TAPE-TO-TAPE COPY PROGRAM.           *   FILE 174
//*      IT USES QSAM, FORCING LABEL=BLP, AND PERFORMS ITS          *   FILE 174
//*      OWN LABEL PROCESSING INTERNALLY.                           *   FILE 174
//*                                                                 *   FILE 174
//*      ATTRIBUTES:                                                *   FILE 174
//*         PROBLEM PROGRAM                                         *   FILE 174
//*         AUTHORIZED (AC=1) *                                     *   FILE 174
//*         NON-REENTRANT                                           *   FILE 174
//*         NONRESIDENT, IN LINKLIB                                 *   FILE 174
//*                                                                 *   FILE 174
//*         * PROGRAM AUTHORIZATION IS REQUIRED IN ORDER TO SET     *   FILE 174
//*            LABEL=BLP VIA OPEN TYPE=J.                           *   FILE 174
//*                                                                 *   FILE 174
//*      HAS BEEN FIXED BY THE AUTHOR TO READ TAPES ON A 3480       *   FILE 174
//*      OR 3480 IDRC DEVICE.  SEEMS GOOD FOR 3490E'S TOO.  I       *   FILE 174
//*      CHECKED THE UCB "HEX" UNIT TYPE FOR 3490E'S  (SBG).        *   FILE 174
//*                                                                 *   FILE 174
//*      SYSTEM LEVEL:  THIS PROGRAM IS BELIEVED TO WORK            *   FILE 174
//*         WITH ALL OPERATING SYSTEM LEVELS FROM OS/MVT            *   FILE 174
//*         THROUGH MVS/ESA.  THE PRIMARY OPERATING SYSTEM          *   FILE 174
//*         DEPENDENCY IS IN DETERMINING THE TAPE UNIT              *   FILE 174
//*         SERIAL NUMBER FOR 34XX TAPE DRIVES, AND THAT            *   FILE 174
//*         CODE IS DUAL-PATHED AS NEEDED.                          *   FILE 174
//*                                                                 *   FILE 174
//*      DISCLAIMER:                                                *   FILE 174
//*                                                                 *   FILE 174
//*       +-------------------------------------------------------+ *   FILE 174
//*       |                                                       | *   FILE 174
//*       | THIS PROGRAM HAS BEEN USED SUCCESSFULLY, AND TO THE   | *   FILE 174
//*       | BEST OF OUR KNOWLEDGE IT IS OPERATIONAL.  HOWEVER, NO | *   FILE 174
//*       | WARRANTY IS MADE TO THE ACCURACY OF THIS PROGRAM OR   | *   FILE 174
//*       | RELATED MATERIAL, AND NO RESPONSIBILITY IS ASSUMED    | *   FILE 174
//*       | FOR ANY MODIFICATION DIRECTLY OR INDIRECTLY CAUSED    | *   FILE 174
//*       | BY THE USE OF THIS PROGRAM.  WHILE WE WOULD LIKE TO   | *   FILE 174
//*       | KNOW OF ANY ERRORS IN THIS PROGRAM, THERE IS NO       | *   FILE 174
//*       | COMMITMENT TO FIX THEM.  THIS PROGRAM IS DISTRIBUTED  | *   FILE 174
//*       | WITHOUT ANY WARRANTIES EITHER EXPRESS OR IMPLIED.     | *   FILE 174
//*       |                                                       | *   FILE 174
//*       +-------------------------------------------------------+ *   FILE 174
//*                                                                 *   FILE 174
~~~~~~~~~~~~~~~~

