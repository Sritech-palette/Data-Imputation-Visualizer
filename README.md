# 📊 Data Imputation Visualizer

*Learn how to fill missing data with pictures!*

## What does this do?

Sometimes your dataset has missing values like when 5 respondents provided their age but one ghosted the survey. This tool demonstrates 3 industry-standard imputation techniques and generates visualizations so you can evaluate performance. It's low-key the MVP for your data preprocessing pipeline.

## Three Ways to Fill Missing Data

1. **Mean (Average)** 

- **What it does:** Adds up all numbers and divides by how many you have  
- **Example:** Ages are 20, 22, 25, 28. Average = 23.75  
- **When to use:** When your numbers are spread out normally  
- **Good for:** Ages, test scores, temperatures

2. **Median (Middle Number)** 

- **What it does:** Finds the number in the middle when you line them up  
- **Example:** Incomes are $30k, $35k, $40k, $5M. Middle = $35k (ignores that crazy high $5M!)  
- **When to use:** When you have some really high or low numbers that don't fit  
- **Good for:** Salaries, house prices, anything with outliers

3. **Mode (Most Frequent)** 

- **What it does:** Picks whatever appears most often  
- **Example:** Colors are Red, Blue, Red, Red, Red. Most popular = Red (appears 4 times)  
- **When to use:** When your data is categories, not numbers  
- **Good for:** Favorite colors, yes/no answers, categories

## Execution on Google Colab 

Folks, I already uploaded the `.ipynb` file for you, no need to copy-paste code or mess around!

Just hit up [Google Colab](https://colab.research.google.com), then simply:

1. Click **File > Open notebook**  
2. Go to the **Upload** tab  
3. Drag & drop the `.ipynb` file I provided.  
4. Wait for it to load (quick AF).  
5. Hit **Runtime > Run all** or smash that play button on each cell . 

Pro tip: The first cell usually installs `matplotlib` and `numpy` with this magic spell:  
```python
!pip install matplotlib numpy

## How to Use This if not Google Colab

### Step 1: Install Python stuff
```bash
pip install matplotlib numpy


## How to Use This

### Step 1: Install Python stuff
```bash
pip install matplotlib numpy
```

### Step 2: Run the code
```bash
python imputation_visualizer.py
```

### Step 3: Look at the charts!
You'll see 3 charts showing each method in action.

## What You'll See

**Chart 1**: Bar chart of ages with a red line showing the average  
**Chart 2**: Bar chart of incomes with an orange line showing the middle value  
**Chart 3**: Bar chart showing how many times each color was picked  

## Why This Matters

Real data is messy! People skip questions, sensors break, files get corrupted. Before you can analyze your data, you need to decide what to do about the missing pieces. This tool helps you see your options.

## Want to Change the Examples?

Look for these lines in the code:
```python
mean_data = [20, 22, 25, 23.75, 28]        # Change these ages
median_data = [30000, 35000, 40000, 35000, 5000000]  # Change these incomes  
mode_data = ['Red', 'Blue', 'Red', 'Red', 'Red']     # Change these colors
```

Put in your own numbers and see what happens!

## Problems?

- **"Module not found"**: Run `pip install matplotlib numpy`
- **Weird looking charts**: Try running it again
- **Code doesn't work**: Make sure you copied all of it

## That's It!

Now you know the 3 basic ways to handle missing data. As you learn more about data science, you'll discover fancier methods, but these 3 are the foundation everything else builds on.

**Happy data cleaning!** 🧹📊
