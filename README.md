# multienv_sim

In the process of refactoring the code to be more modular and easier to setup.

TODO:
- [x] gym-pybullet-drones working in its self-contained repo
- [x] drone_causality working in its self-contained repo
- [ ] gaussian-splatting working in its self-contained repo
- [ ] create general scripts to work cross repos (in multienv sim)
- [ ] use configs in multienv_sim repo to start scripts

## Setup
```bash
export PYTHONPATH=$PYTHONPATH:$(pwd)/pybullet_env
export PYTHONPATH=$PYTHONPATH:$(pwd)/drone_causality
export PYTHONPATH=$PYTHONPATH:$(pwd)/gaussian_splatting
```

## PyBullet Synthetic Environment
### Generating Data
```python
python pybullet_env/scripts/generate_synthetic_trajectories.py
```
 
### Evaluation
```python
python pybullet_env/scripts/evaluate_policy.py
```