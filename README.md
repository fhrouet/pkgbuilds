# pkgbuilds
Arch Linux pkgbuilds for some scientific packages:
 - OpenBLAS     0.2.14
 - ScaLAPACK    2.0.2 
 - Scotch       6.0.4
 - ParMETIS     4.0.3
 - MUMPS        5.0.1
 - SuperLU_DIST 4.1
 - FFTW         3.3.4
 - PETSc        3.6.1
 - PAPI         5.4.1

Notes:
 - OpenBLAS is compiled with USE_OPENMP=1. It provides both lapack and blas.
 - Scotch is compiled without SCOTCH_PTHREAD (so that it plays nicely with MPI).
 - ParMETIS provides both metis and parmetis.
 - Scotch provides both scotch and ptscotch.
 - MUMPS is compiled with METIS, ParMETIS, Scotch and PT-Scotch options enabled. It's an MPI version (not dummy MPI).
 - FFTW is compiled with MPI support.
 - PETSc is compiled with ParMETIS, Scotch, MUMPS, SuperLU_DIST options enabled. 

The packages rely on the GNU compilers (gcc/gfortran/g++), OpenMP from gcc-libs, and MPI from the openmpi package.

Links:
 - OpenBLAS      http://github.com/xianyi/OpenBLAS/
                 http://github.com/xianyi/OpenBLAS/archive/v0.2.14.tar.gz
 - ScaLAPACK     http://www.netlib.org/scalapack/
                 http://www.netlib.org/scalapack/scalapack-2.0.2.tgz
 - Scotch        http://gforge.inria.fr/projects/scotch/ 
                 http://gforge.inria.fr/frs/download.php/file/34618/scotch_6.0.4.tar.gz
 - ParMETIS      http://glaros.dtc.umn.edu/gkhome/metis/parmetis/overview
                 http://glaros.dtc.umn.edu/gkhome/fetch/sw/parmetis/parmetis-4.0.3.tar.gz
 - MUMPS         http://mumps.enseeiht.fr
                 http://mumps.enseeiht.fr/MUMPS_5.0.1.tar.gz
 - SuperLU_DIST  http://crd-legacy.lbl.gov/~xiaoye/SuperLU/#superlu_dist
                 http://crd-legacy.lbl.gov/~xiaoye/SuperLU/superlu_dist_4.1.tar.gz
 - FFTW          http://www.fftw.org
                 http://www.fftw.org/fftw-3.3.4.tar.gz
 - PETSc         http://www.mcs.anl.gov/petsc/
                 http://ftp.mcs.anl.gov/pub/petsc/release-snapshots/petsc-lite-3.6.1.tar.gz
 - PAPI          http://icl.cs.utk.edu/papi/index.html
                 http://icl.cs.utk.edu/projects/papi/downloads/papi-5.4.1.tar.gz
