# Saving a Model Made in fastai

Training can take a lot of computational time. Ideally, we would be able to save our models so that we can accss them later without having to retrain a new one. This saves a lot of time and effort. Luckily, the fastai library allows this to be done quickly and easily.
So first we need to train a model, this is the basic training process described throughout the course (this assumes you already have your data blocks set up):
```python
learn = vision_learner(dls, resnet18, metrics=error_rate)
learn.fine_tune(3)
```
Now that we have a model stored as a *Learner* type it can be exported as a .plk

```python
learn.export('model.pkl')
```

The file should appear in the directory you are currently working in. There are a number of ways to download/save it. One is by adding it to your git repository and pushing it out. That should save it so that it will be ready to go next time you need it. Obviously now that we have exported a model we want to be able to import one. This is quick and easy.

```python
learn = load_learner('model.pkl')
```

The model is now an environemnt variable that you can use for predictions, testing or further training.

This has been adapted from [fastai lesson 2](https://course.fast.ai/Lessons/lesson2.html)
