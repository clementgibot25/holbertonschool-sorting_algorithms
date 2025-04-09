# Sorting Algorithms in C

This repository provides implementations of common sorting algorithms in the C programming language. Each algorithm is accompanied by a brief explanation and its time and space complexity in Big O notation.

## 📌 What is Big O Notation?

Big O notation describes the performance or complexity of an algorithm in terms of time (execution speed) or space (memory usage) as the input size grows.

| Notation   | Name         | Description                                 |
|------------|--------------|---------------------------------------------|
| O(1)       | Constant     | Execution time doesn't depend on input size |
| O(log n)   | Logarithmic  | Grows slowly with input size                |
| O(n)       | Linear       | Grows directly with input size              |
| O(n log n) | Linearithmic | Efficient for large datasets                |
| O(n²)      | Quadratic    | Slower, suitable for small datasets         |

---

## 🧮 Sorting Algorithms

### 1. **Bubble Sort**
- **Description**: Repeatedly swaps adjacent elements if they are in the wrong order.
- **Best Case**: O(n) — already sorted
- **Average/Worst Case**: O(n²)
- **Space**: O(1) (in-place)

```c
void bubble_sort(int arr[], int n);
```

---

### 2. **Selection Sort**
- **Description**: Repeatedly selects the smallest (or largest) element and moves it to the sorted part of the array.
- **Time Complexity**: O(n²)
- **Space**: O(1)

```c
void selection_sort(int arr[], int n);
```

---

### 3. **Insertion Sort**
- **Description**: Builds the final sorted array one element at a time.
- **Best Case**: O(n) — nearly sorted
- **Average/Worst Case**: O(n²)
- **Space**: O(1)

```c
void insertion_sort(int arr[], int n);
```

---

### 4. **Merge Sort**
- **Description**: Divide and conquer algorithm. Divides the array into halves, sorts and merges them.
- **Time Complexity**: O(n log n) for all cases
- **Space**: O(n) (not in-place)

```c
void merge_sort(int arr[], int left, int right);
```

---

### 5. **Quick Sort**
- **Description**: Divide and conquer. Picks a pivot and partitions the array around it.
- **Best/Average Case**: O(n log n)
- **Worst Case**: O(n²) — when the smallest or largest element is always chosen as pivot
- **Space**: O(log n)

```c
void quick_sort(int arr[], int low, int high);
```

---

### 6. **Heap Sort**
- **Description**: Converts array into a heap and repeatedly extracts the max element.
- **Time Complexity**: O(n log n)
- **Space**: O(1)

```c
void heap_sort(int arr[], int n);
```

---

## 🧪 How to Compile and Run

```bash
gcc -o sort main.c
./sort
```

Make sure to include the correct sorting algorithm's `.c` and `.h` file in your `main.c`.

---

## 📂 Example Project Structure

```
sorting-project/
├── bubble_sort.c
├── insertion_sort.c
├── merge_sort.c
├── quick_sort.c
├── selection_sort.c
├── heap_sort.c
├── sort_utils.h
├── main.c
└── README.md
```

---
## Authors

- Arnaud TILAWAT / Clément GIBOT