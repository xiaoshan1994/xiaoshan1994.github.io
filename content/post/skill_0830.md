---
title: "Creating multiple subplots using plt.subplots"
date: 2021-08-30T11:31:15+02:00
description:
images:
- https://cdn.educba.com/academy/wp-content/uploads/2020/07/psd-9-1-2-2.jpg
thumbnailImagePosition: left
thumbnailImage: //cdn.educba.com/academy/wp-content/uploads/2020/07/psd-9-1-2-2.jpg
tags:
- python
- matplotlib
Categories:
- Skill
- Academic Drawing
---
pyplot.subplots creates a figure and a grid of subplots with a single call, while providing reasonable control over how the individual plots are created. For more advanced use cases you can use GridSpec for a more general subplot layout or Figure.add_subplot for adding subplots at arbitrary locations within the figure.
https://matplotlib.org/stable/gallery/subplots_axes_and_figures/subplots_demo.html

[matplotlib.pyplot.subplots](https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.subplots.html#matplotlib.pyplot.subplots)
matplotlib.pyplot.subplots(nrows=1, ncols=1, *, sharex=False, sharey=False, squeeze=True, subplot_kw=None, gridspec_kw=None, **fig_kw)

Returns:
`fig`: The matplotlib.pyplot.figure object to be used as a **container** for all the subplots.
`ax`: A single object of the axes. Axes object if there is only **one plot**, or **an array of axes**. Axes objects if there are multiple plots, as specified by the nrows and ncols.

Typical idioms for handling the return value are:
Using the variable ax for single a Axes
```
fig, ax = plt.subplots()
```
Using the variable axs for multiple Axes
```
fig, axs = plt.subplots(2, 2)
```
Using tuple unpacking for multiple Axes
```
fig, (ax1, ax2) = plt.subplots(1, 2)
fig, ((ax1, ax2), (ax3, ax4)) = plt.subplots(2, 2)
```
### A figure with just one subplot
```
import matplotlib.pyplot as plt
import numpy as np

## Some example data to display
x = np.linspace(0, 2 * np.pi, 400)
y = np.sin(x ** 2)
```
```
fig, ax = plt.subplots()
ax.plot(x,y)
ax.set_title('A single plot')
```
![image](https://user-images.githubusercontent.com/65668613/131475906-69dd85ff-bcbb-4288-a24e-cf2b9295dfce.png)

### Stacking subplots in one direction
```
fig,ax = plt.subplots(2)
fig.subtitle('Vertically stacked subplots')
axs[0].plot(x,y)
axs[1].plot(x,-y)
```
![image](https://user-images.githubusercontent.com/65668613/131477410-d915bb0d-cc24-456a-8c72-bab48296ff5a.png)

If you are creating just a few Axes, it's handy to unpack them immediately to dedicated variables for each Axes. That way, we can use ax1 instead of the more verbose axs[0].

```
fig, (ax1,ax2) = plt.subplots(2)
fig.suptitle('Vertically stacked subplots')
ax1.plot(x, y)
ax2.plot(x, -y)
```
![image](https://user-images.githubusercontent.com/65668613/131477875-586ceb55-220a-49a8-8f81-4be319c12bad.png)

To obtain side-by-side subplots, pass parameters 1, 2 for one row and two columns.
```
fig, (ax1,ax2) = plt.subplots(1,2)
fig.subtitle('Horizontally stacked subplots')
ax1.plot(x,y)
ax2.plot(x,-y)
```
![image](https://user-images.githubusercontent.com/65668613/131478295-c31e785f-e621-4c57-96c6-e9c478087212.png)

### Stacking subplots in two directions
When stacking in two directions, the returned `axs` is a 2D NumPy array.
If you have to set parameters for each subplot it's handy to iterate over all subplots in a 2D grid using `for ax in axs.flat`:
```
fig,axs = plt.subplots(2,2)
axs[0,0].plot(x,y)
axs[0,0].set_title('Axis [0, 0]')
axs[0,1].plot(x,y,'tab:orange')
axs[0,1].set_title('Axis [0, 1]')
axs[1,0].plot(x, -y, 'tab:green')
axs[1,0].set_title('Axis [1, 0]')
axs[1,1].plot(x, -y, 'tab:red')
axs[1,1].set_title('Axis [1, 1]')

for ax in axs.flat:
ax.set(xlabel='x-label',ylabel='y-label')

# Hide x labels and tick labels for top plots and y ticks for right plots.
for ax in axs.flat:
    ax.label_outer() # Only show "outer" labels and tick labels. x-labels are only kept for subplots on the last row; y-labels only for subplots on the first column.
```
![image](https://user-images.githubusercontent.com/65668613/131483362-8726e2b9-631a-40cf-b78b-72dc71beca98.png)

You can use tuple-unpacking also in 2D to assign all subplots to dedicated variables:
> In python tuples are used to store immutable objects. In packing, we put values into a new tuple while in unpacking we extract those values into a single variable.
Packing: a = ("MNNIT Allahabad", 5000, "Engineering"),
Unpacking: (college, student, type_ofcollege) = a.
```
fig,((ax1,ax2),(ax3,ax4)) = plt.subplots(2,2)
fig.suptitle('Sharing x per column, y per row')
ax1.plot(x,y)
ax2.plot(x,y**2,'tab:orange')
ax3.plot(x,-y,'tab:green')
ax4.plot(x, -y**2, 'tab:red')
for ax in fig.get_axes():
ax.label_outer()
```
![image](https://user-images.githubusercontent.com/65668613/131642513-eff75765-a38b-4435-9e2f-7f19af2c0fa2.png)

### Sharing axes
By default, each Axes is scaled individually. Thus, if the ranges are different the tick values of the subplots do not align.
```
fig, (ax1, ax2) = plt.subplots(2)
fig.suptitle('Axes values are scaled individually by default')
ax1.plot(x, y)
ax2.plot(x + 1, -y)
```
![image](https://user-images.githubusercontent.com/65668613/131644381-699d2759-d34d-4f97-806d-5f0aae2653b5.png)

You can use sharex or sharey to align the horizontal or vertical axis.
```
fig, (ax1, ax2) = plt.subplots(2, sharex=True)
fig.suptitle('Aligning x-axis using sharex')
ax1.plot(x, y)
ax2.plot(x + 1, -y)
```
![image](https://user-images.githubusercontent.com/65668613/131644328-ebcdf740-902e-4989-b819-9a9e4f1b3fe5.png)

Setting sharex or sharey to `True` enables global sharing across the whole grid, i.e. also the y-axes of vertically stacked subplots have the same scale when using sharey = `True`.
```
fig, axs = plt.subplots(3, sharex= True, sharey= True)
fig.suptitle('Sharing both axes')
axs[0].plot(x, y ** 2)
axs[1].plot(x, 0.3 * y, 'o')
axs[2].plot(x, y, '+')
```
![image](https://user-images.githubusercontent.com/65668613/131645322-d62a6c81-fdff-40d4-963e-f8ec8b173588.png)

For subplots that are sharing axes one set of tick labels is enough. Tick labels of inner Axes are automatically removed by sharex and sharey. Still there remains an unused empty space between the subplots.

To precisely control the positioning of the subplots, one can explicitly create a `GridSpec` with `Figure.add_gridspec`, and then call its `subplots` method. For example, we can reduce the height between vertical subplots using `add_gridspec(hspace=0)`.

`label_outer` is a handy method to remove labels and ticks from subplots that are not at the edge of the grid.
```
fig = plt.figure()
gs = fig.add_gridspec(3, hspace=0)
axs = gs.subplots(sharex= True, sharey = True)
fig.suptitle('Sharing both axes')
fig.suptitle('Sharing both axes')
axs[0].plot(x, y ** 2)
axs[1].plot(x, 0.3 * y, 'o')
axs[2].plot(x, y, '+')
```
![image](https://user-images.githubusercontent.com/65668613/131649016-9975c4c0-402a-449c-8f8c-0e76b46baa9f.png)

Apart from `True` and `False`, both `sharex` and `sharey` accept the values 'row' and 'col' to share the values only per row or column.
```
fig = plt.figure()
gs = fig.add_gridspec(2,2,hspace=0,wspace=0)
(ax1,ax2),(ax3,ax4) = gs.subplots(sharex='col', sharey = 'row')
fig.suptitle('Sharing x per column, y per row')
ax1.plot(x, y)
ax2.plot(x, y**2, 'tab:orange')
ax3.plot(x + 1, -y, 'tab:green')
ax4.plot(x + 2, -y**2, 'tab:red')
for ax in axs.flat:
ax.label_outer()
```
![image](https://user-images.githubusercontent.com/65668613/131649828-b7ab90f6-7a7b-444a-abd1-69dc97ba93c6.png)

If you want a more complex sharing structure, you can first create the grid of axes with no sharing, and then call `axes.Axes.sharex` or `axes.Axes.sharey` to add sharing info a posteriori.
```go {linenos= false,hl_lines=[6],linenostart=184}
fig, axs = plt.subplots(2, 2)
axs[0, 0].plot(x, y)
axs[0, 0].set_title("main")
axs[1, 0].plot(x, y**2)
axs[1, 0].set_title("shares x with main")
axs[1, 0].sharex(axs[0, 0])
axs[0, 1].plot(x + 1, y + 1)
axs[0, 1].set_title("unrelated")
axs[1, 1].plot(x + 2, y + 2)
axs[1, 1].set_title("also unrelated")
fig.tight_layout() // narrowing the padding between figure edge and edges of the subplots
```
![image](https://user-images.githubusercontent.com/65668613/131653973-f49b697d-1db1-4ae0-a6fa-498b44fb6d2c.png)

### Polar axes
The parameter ***subplot_kw*** of `pyplot.subplots` controls the subplot properties (see also `Figure.add_subplot`). In particular, this can be used to create a grid of polar Axes.
```
fig, (ax1, ax2) = plt.subplots(1, 2, subplot_kw=dict(projection='polar'))
ax1.plot(x, y)
ax2.plot(x, y ** 2)

plt.show()
```
![image](https://user-images.githubusercontent.com/65668613/131653802-efa8c7fd-8cba-4e9c-bc8f-c1f060d3fb76.png)
