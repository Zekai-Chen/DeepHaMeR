# DeepHaMeR

Create a 3D hand mesh recovery model that is better than HaMeR https://github.com/geopavlakos/hamer
HaMeR is a transformer-based single-image 3D hand mesh recovery model, usually used inside a hand reconstruction pipeline
Hand crop image
→ Vision Transformer backbone
→ Transformer decoder / regression head
→ MANO parameters + camera
→ MANO mesh and joints

The HaMeR https://github.com/geopavlakos/hamer use bash fetch_training_data.sh to get all the training data and train with python train.py exp_name=hamer data=mix_all experiment=hamer_vit_transformer trainer=gpu launcher=local

For the perfromance, you can refer to HaMeR GitHub eval pipeline (main focus) FreiHAND benchmark / leaderboard https://github.com/lmb-freiburg/freihand?utm_source=chatgpt.com, HO-3D / Codalab evaluation ,HInt evaluation ,HyperAI https://vercel.hyper.ai/en/sota/tasks/3d-hand-pose-estimation/benchmark/3d-hand-pose-estimation-on-freihand?utm_source=chatgpt.com to compare

Try on the given H100 80GB first， REPORT to me if you need more powerful compute resources
