# 6.2 GPU usage

### **Training task & jobs**

Users can set up a training task by selecting training data, model & tuning method. For better tuning efficiency, there might be multiple parallel training jobs within one training task, **each job runs on a specific set of hyperparameter and will occupy 1 GPU each**. The training time of each job depends on the GPU spec, model property, data size & other settings such as early stop. A training task will be complete once all training jobs are finished.

&#x20;                                         ![](<../.gitbook/assets/image (13).png>)

**Manual assignment**

Given a specific set of hyperparameter, manual assignment task will only run one job.

![](<../.gitbook/assets/image (10).png>)

**Grid search**

The number of jobs in grid search is determined by the number of search points in hyperparameter space. The total numbers of jobs is limited to 48 job max.

![](<../.gitbook/assets/image (204).png>)

The total number of jobs (search points) = “# of learning rate x # of weight decays x # of momentum”

![](<../.gitbook/assets/image (181).png>)

An error will appear if the number of jobs exceed 48, this task cannot be started unless the numbers are fixed.

**Random search**

Random search runs multiple jobs with random hyperparameter combination within the given range (min-max of each hyperparameter), the min. number of jobs is 8 and the max number of jobs is 48.

![](<../.gitbook/assets/image (192).png>)

**Population based tuning**

PBT also runs multiple jobs with different hyperparameter combination within the given range (min-max of each hyperparameter), where the DeepQ AutoML engine will search for the optimal hyperparameter adaptively. The min. number of jobs is 8 and the max number of jobs is 48. (Default setting of DeepQ AutoML is PBT-24 jobs)

![](<../.gitbook/assets/image (167).png>)

![Tuning methods and jobs/GPUs](<../.gitbook/assets/image (152).png>)
