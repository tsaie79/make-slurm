apptainer exec --env SLURM_CONF=$HOME/slurm.conf --bind /run/munge/munge.socket.2:/run/munge/munge.socket.2 slurm_v0.1.sif bash

shifter --image=jlabtsai/slurm:v0.1 --env=SLURM_CONF=$HOME/slurm.conf  -- bash

