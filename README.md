# SPECFEM3D-Modify

Attempt No.1
Rewrite the 

1.LATITUDE_MAX  = 288.00    into.   .LATITUDE_MAX  = 40.00.   
  LONGITUDE_MAX = 144.00             LONGITUDE_MAX = 40.00
  
2.SPACING_XI    = 288.00.   into     SPACING_XI.   = 40.00
  SPACING_ETA   = 144.00             SPACING_ETA   = 40.00

Results: WRONG!!!
******************************************************************************************************************************
  running solver on  2 processors...

 need at least one receiver
 Error detected, aborting MPI... proc            0
 need at least one receiver
 Error detected, aborting MPI... proc            1
--------------------------------------------------------------------------
MPI_ABORT was invoked on rank 0 in communicator MPI_COMM_WORLD
with errorcode 30.

NOTE: invoking MPI_ABORT causes Open MPI to kill all MPI processes.
You may or may not see output from other processes, depending on
exactly when Open MPI kills them.
--------------------------------------------------------------------------
[bixie1:06774] 1 more process has sent help message help-mpi-api.txt / mpi-abort
[bixie1:06774] Set MCA parameter "orte_base_help_aggregate" to 0 to see all help / error messages
******************************************************************************************************************************




Attempt No.2
Reweite the LATITUDE & LOTITUDE back.

Results:
******************************************************************************************************************************
run_this_example.sh:行99: ./bin/xcreate_movie_shakemap_AVS_DX_GMT: 没有那个文件或目录
******************************************************************************************************************************
