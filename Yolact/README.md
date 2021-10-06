# YOLACT Real-time Instance Segmentation :- 

![image](https://user-images.githubusercontent.com/76057253/136133054-2ef46a61-1f60-4b60-9211-df98eb0acbed.png)


Pytorch implementation of Yolact .

## Abstract :- 
We present a simple, fully-convolutional model for realtime instance segmentation that achieves 29.8 mAP on MS
COCO at 33.5 fps evaluated on a single Titan Xp, which is
significantly faster than any previous competitive approach.
Moreover, we obtain this result after training on only one
GPU. We accomplish this by breaking instance segmentation into two parallel subtasks: (1) generating a set of prototype masks and (2) predicting per-instance mask coefficients. Then we produce instance masks by linearly combining the prototypes with the mask coefficients. We find that
because this process doesn’t depend on repooling, this approach produces very high-quality masks and exhibits temporal stability for free. Furthermore, we analyze the emergent behavior of our prototypes and show they learn to localize instances on their own in a translation variant manner, despite being fully-convolutional. Finally, we also propose Fast NMS, a drop-in 12 ms faster replacement for standard NMS that only has a marginal performance penalty.

## Architecture :- 
![image](https://user-images.githubusercontent.com/76057253/136132944-3ce48e8b-8fc0-45b4-93bc-b580042211d9.png)

### Prototypes :-
![image](https://user-images.githubusercontent.com/76057253/136133281-d41cce11-ef8f-4d49-8919-1fe8a811834b.png)


## Results :- 


### Mask mAP VS FPS :- 
![image](https://user-images.githubusercontent.com/76057253/136133018-32165482-5e3d-45aa-8390-cce01ae4d44c.png)

![image](https://user-images.githubusercontent.com/76057253/136133073-8fb4db3b-f0f2-408b-9872-e1126004defd.png)
![image](https://user-images.githubusercontent.com/76057253/136132989-0fb25eee-a702-457b-87a1-7f4c18eadd0b.png)

```
@misc{bolya2019yolact,
      title={YOLACT: Real-time Instance Segmentation}, 
      author={Daniel Bolya and Chong Zhou and Fanyi Xiao and Yong Jae Lee},
      year={2019},
      eprint={1904.02689},
      archivePrefix={arXiv},
      primaryClass={cs.CV}
}
```
