Commands to execute OpenMP programs:



Get necessary packages (one time step

      sudo apt-get update
      audo apt-get upgrade
      sudo apt-get install libopenmpi-dev libgd-dev
     
To compile and run codes:
  
      gcc <filename>.c -fopenmp -lgd -lm
      ./a.out
      
      
      
      
      
      
 Commands to execute MPI programs:


Get necessary packages and setup (one time step):

      sudo apt-get install mpich mpich-doc
      sudo update-alternatives --config mpi #you may need to select a certain MPI installation

To compile and run codes:

      mpicc <filename>.c
      mpirun -np 4 ./a.out 
      #try mpiexec if mpirun does not work
      #try with -np 2 if 4 does not work
