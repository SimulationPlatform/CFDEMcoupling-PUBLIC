# Install notes on CFDEMcoupling-PUBLIC

## System
Tested on Ubuntu 15.10 x86_64.

## Environment variables


```bash
# Source LIGGGHTS variables
alias liggghts="$HOME/LIGGGHTS/LIGGGHTS-PUBLIC/src/lmp_fedora_fpic"
export LPP_DIR=$HOME/LIGGGHTS/LPP/src
export LPP_NPROCS=4
export LPP_CHUNKSIZE=1
alias lpp='python -i $LPP_DIR/lpp.py --cpunum $LPP_NPROCS --chunksize
$LPP_CHUNKSIZE'
```

```bash
# Source CFDEM variables

export CFDEM_VERSION=PUBLIC
export
CFDEM_PROJECT_DIR=$HOME/CFDEM/CFDEMcoupling-$CFDEM_VERSION-$WM_PROJECT_VERSION
export CFDEM_SRC_DIR=$CFDEM_PROJECT_DIR/src
export CFDEM_SOLVER_DIR=$CFDEM_PROJECT_DIR/applications/solvers
export CFDEM_DOC_DIR=$CFDEM_PROJECT_DIR/doc
export CFDEM_UT_DIR=$CFDEM_PROJECT_DIR/applications/utilities
export CFDEM_TUT_DIR=$CFDEM_PROJECT_DIR/tutorials
export
CFDEM_PROJECT_USER_DIR=$HOME/CFDEM/$LOGNAME-$CFDEM_VERSION-$WM_PROJECT_VERSION
export CFDEM_bashrc=$CFDEM_SRC_DIR/lagrangian/cfdemParticle/etc/bashrc
export CFDEM_LIGGGHTS_SRC_DIR=$HOME/LIGGGHTS/LIGGGHTS-PUBLIC/src
export CFDEM_LIGGGHTS_MAKEFILE_NAME=fedora_fpic
export CFDEM_LPP_DIR=$HOME/LIGGGHTS/LPP/src
export CFDEM_PIZZA_DIR=$HOME/LIGGGHTS/LPP/src
. $CFDEM_bashrc
```
