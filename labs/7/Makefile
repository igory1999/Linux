t1:
	sbatch t1.batch
t2:
	sbatch t2.batch
mon:
	watch squeue -u $(USER)
clean:
	rm -f *.out *.err *~
