# عنوان درس: ساختمان داده

### توضیحات کلی:

مطالب این فایل شامل نکات و جزوات مرتبط با درس ساختمان داده است.

## فصل 1: آشنایی با ساختمان داده

- تعریف: ساختمان داده گروهی از عناصر داده است که ساده‌ترین راه را برای ذخیره و انجام اقدامات مختلف بر روی‌داده‌های کامپیوتر را فراهم می‌کند.

  ![Data Structure](https://media.geeksforgeeks.org/wp-content/cdn-uploads/20230706095706/intro-data-structure-%E2%80%93-1.png)

### انواع ساختمان داده‌ها:

- **ساختمان داده خطی**: ساختمان داده خطی که در آن عناصر داده به‌صورت متوالی یا خطی ‌مرتب‌شده‌اند، جایی که هر عنصر به عناصر مجاور قبلی و بعدی خود متصل می‌شود، ساختمان داده خطی نامیده می‌شود. نمونه‌هایی از ساختارهای داده خطی عبارت‌اند از: آرایه، پشته، صف، لیست پیوندی و غیره.
- **ساختمان داده ایستا**:
  ساختمان داده استاتیک دارای اندازه حافظه ثابت است. دسترسی به عناصر در یک ساختمان داده ‌ایستا آسان‌تر از ساختمان داده خطی به‌حساب می‌آید. نمونه‌ای از این ساختمان داده، آرایه است.
- **ساختمان داده پویا**:
  در ساختمان داده پویا، اندازه ثابت نیست و ممکن است که به‌طور تصادفی در طول زمان اجرا به‌روز شود. نمونه‌هایی از این ساختمان داده عبارت‌اند از: صف، پشته و غیره.
- **ساختمان داده غیر خطی**:
  در ساختارهای داده غیر خطی، عناصر داده به‌صورت متوالی یا خطی قرار نمی‌گیرند. نمونه‌هایی از ساختارهای داده غیرخطی درختان و نمودارها هستند.

### انواع داده ساختارها:

- شکل‌های مختلفی برای ذخیره داده وجود دارد که در دوره آموزش ساختمان داده به آن پرداخته‌شده است. در ادامه مروری بر برخی از ساختارهای داده رایج خواهیم داشت.

![Calssification](https://media.geeksforgeeks.org/wp-content/uploads/20220520182504/ClassificationofDataStructure-660x347.jpg)

- **آرایه**:آرایه مجموعه‌ای از اقلام داده‌ای است که در مکان‌های حافظه به‌هم‌پیوسته ذخیره می‌شوند. ایده آرایه این است که چندین مورد از یک نوع را با هم ذخیره کند. این کار محاسبه موقعیت هر عنصر را با افزودن یک افست به یک مقدار پایه، یعنی مکان حافظه اولین عنصر آرایه (که معمولاً بانام آرایه مشخص می‌شود) آسان‌تر می‌کند.
- **لیست پیوندی**:مانند آرایه‌ها، لیست پیوندی نوعی ساختمان داده خطی به‌حساب می‌آید که در دوره آموزش ساختمان داده مکتب خونه به‌صورت کامل جنبه‌های مختلف آن پوشش داده‌شده است. برخلاف آرایه‌ها، عناصر لیست پیوندی در مکانی پیوسته ذخیره نمی‌شوند. عناصر با استفاده از اشاره‌گر به هم مرتبط می‌شوند.

- **صف**:صف نوعی ساختار خطی دارد که از ترتیب خاصی پیروی می‌کند که در آن عملیات انجام می‌شود. ترتیب اولین خروجی (FIFO) است. در صف، آیتم‌ها در یک انتها درج می‌شوند و از انتهای دیگر حذف می‌شوند. در دوره آموزش ساختمان داده ما با صف و انواع عملیات روی آن آشنا خواهیم شد.
- **پشته**: پشته نوعی ساختمان داده خطی است که از ترتیب خاصی پیروی می‌کند که در آن عملیات انجام می‌شود. سفارش ممکن است LIFO (آخرین در اولین خروج) یا FILO (اول در آخرین خروج) باشد. در پشته، تمام درج و حذف فقط در یک انتهای لیست مجاز است.
- **درخت دودویی**:برخلاف آرایه‌ها، لیست‌های پیوندی، پشته و صف‌ها که ساختارهای داده خطی هستند، درخت‌ها ساختارهای داده سلسله مراتبی هستند. درخت باینری یا درخت دودویی نوعی ساختمان داده درختی است که در آن هر گره حداکثر دو فرزند دارد که به آن‌ها فرزند چپ و فرزند راست گفته می‌شود. عمدتاً با استفاده از پیوندها اجرا می‌شود. در دوره آموزش ساختمان داده ما با انواع درخت و عملیات مختلف روی آن‌ها آشنا خواهیم شد.

- **گراف**:گراف نوعی ساختمان داده غیرخطی به‌حساب می‌آید که از رئوس (یا گره‌ها) و یال‌ها تشکیل‌شده است. در واقع گراف از مجموعه محدودی از رأس‌ها و مجموعه‌ای از لبه‌ها تشکیل‌شده است که یک جفت گره را به هم متصل می‌کند. گراف برای حل چالش‌برانگیزترین و پیچیده‌ترین مسائل برنامه‌نویسی استفاده می‌شود. اصطلاحات مختلفی در گراف وجود دارد که عبارت‌اند از: مسیر، درجه، رئوس مجاور و غیره.

## فصل 2: انواع مرتب سازی‌ها

### مرتب سازی‌ها:

#### مرتب سازی حبابی (bubble sort):

- ```java class GFG {

     static void bubbleSort(int arr[], int n){
        int i, j, temp;
        boolean swapped;
        for (i = 0; i < n - 1; i++) {
            swapped = false;
            for (j = 0; j < n - i - 1; j++) {
                if (arr[j] > arr[j + 1]) {

                    // Swap arr[j] and arr[j+1]
                    temp = arr[j];
                    arr[j] = arr[j + 1];
                    arr[j + 1] = temp;
                    swapped = true;
                }
            }

            // If no two elements were
            // swapped by inner loop, then break
            if (swapped == false)
                break;
        }
    }

    // Function to print an array
    static void printArray(int arr[], int size){
        int i;
        for (i = 0; i < size; i++)
            System.out.print(arr[i] + " ");
        System.out.println();
    }

    // Driver program
    public static void main(String args[]){
        int arr[] = { 64, 34, 25, 12, 22, 11, 90 };
        int n = arr.length;
        bubbleSort(arr, n);
        System.out.println("Sorted array: ");
        printArray(arr, n);
    }}

  ```

#### مرتب سازی ادغامی (merge sort):

```java

class GfG {

    // Merges two subarrays of arr[].
    // First subarray is arr[l..m]
    // Second subarray is arr[m+1..r]
    static void merge(int arr[], int l, int m, int r)
    {
        // Find sizes of two subarrays to be merged
        int n1 = m - l + 1;
        int n2 = r - m;

        // Create temp arrays
        int L[] = new int[n1];
        int R[] = new int[n2];

        // Copy data to temp arrays
        for (int i = 0; i < n1; ++i)
            L[i] = arr[l + i];
        for (int j = 0; j < n2; ++j)
            R[j] = arr[m + 1 + j];

        // Merge the temp arrays

        // Initial indices of first and second subarrays
        int i = 0, j = 0;

        // Initial index of merged subarray array
        int k = l;
        while (i < n1 && j < n2) {
            if (L[i] <= R[j]) {
                arr[k] = L[i];
                i++;
            }
            else {
                arr[k] = R[j];
                j++;
            }
            k++;
        }

        // Copy remaining elements of L[] if any
        while (i < n1) {
            arr[k] = L[i];
            i++;
            k++;
        }

        // Copy remaining elements of R[] if any
        while (j < n2) {
            arr[k] = R[j];
            j++;
            k++;
        }
    }

    // Main function that sorts arr[l..r] using
    // merge()
    static void sort(int arr[], int l, int r)
    {
        if (l < r) {

            // Find the middle point
            int m = l + (r - l) / 2;

            // Sort first and second halves
            sort(arr, l, m);
            sort(arr, m + 1, r);

            // Merge the sorted halves
            merge(arr, l, m, r);
        }
    }

    // A utility function to print array of size n
    static void printArray(int arr[])
    {
        int n = arr.length;
        for (int i = 0; i < n; ++i)
            System.out.print(arr[i] + " ");
        System.out.println();
    }

    // Driver code
    public static void main(String args[])
    {
        int arr[] = { 12, 11, 13, 5, 6, 7 };

        System.out.println("Given array is");
        printArray(arr);

        sort(arr, 0, arr.length - 1);

        System.out.println("\nSorted array is");
        printArray(arr);
    }
  }
```

```java
Output:

Given array is
12 11 13 5 6 7

Sorted array is
5 6 7 11 12 13

```

#### مرتب سازی انتخابی (selection sort):

```java
static void selectionSort(int[] arr){
        int n = arr.length;
        for (int i = 0; i < n - 1; i++) {

            // Assume the current position holds
            // the minimum element
            int min_idx = i;

            // Iterate through the unsorted portion
            // to find the actual minimum
            for (int j = i + 1; j < n; j++) {
                if (arr[j] < arr[min_idx]) {

                    // Update min_idx if a smaller element
                    // is found
                    min_idx = j;
                }
            }

            // Move minimum element to its
            // correct position
            int temp = arr[i];
            arr[i] = arr[min_idx];
            arr[min_idx] = temp;
        }
    }

    static void printArray(int[] arr){
        for (int val : arr) {
            System.out.print(val + " ");
        }
        System.out.println();
    }

    public static void main(String[] args){
        int[] arr = { 64, 25, 12, 22, 11 };

        System.out.print("Original array: ");
        printArray(arr);

        selectionSort(arr);

        System.out.print("Sorted array: ");
        printArray(arr);
    }
```

```java
- Output: Original vector: 64 25 12 22 11
  Sorted vector: 11 12 22 25 64
```

#### مرتب سازی درجی (insertion sort):

```java
// Java program for implementation of Insertion Sort
public class InsertionSort {
    /* Function to sort array using insertion sort */
    void sort(int arr[])
    {
        int n = arr.length;
        for (int i = 1; i < n; ++i) {
            int key = arr[i];
            int j = i - 1;

            /* Move elements of arr[0..i-1], that are
               greater than key, to one position ahead
               of their current position */
            while (j >= 0 && arr[j] > key) {
                arr[j + 1] = arr[j];
                j = j - 1;
            }
            arr[j + 1] = key;
        }
    }

    /* A utility function to print array of size n */
    static void printArray(int arr[])
    {
        int n = arr.length;
        for (int i = 0; i < n; ++i)
            System.out.print(arr[i] + " ");

        System.out.println();
    }

    // Driver method
    public static void main(String args[])
    {
        int arr[] = { 12, 11, 13, 5, 6 };

        InsertionSort ob = new InsertionSort();
        ob.sort(arr);

        printArray(arr);
    }
}

```

```java
- Output:`5 6 11 12 13 `
```

#### مرتب سازی هرمی (heap sort):

```java
import java.util.Arrays;



    // To heapify a subtree rooted with node i
    // which is an index in arr[].
    static void heapify(int arr[], int n, int i) {

        // Initialize largest as root
        int largest = i;

        // left index = 2*i + 1
        int l = 2 * i + 1;

        // right index = 2*i + 2
        int r = 2 * i + 2;

        // If left child is larger than root
        if (l < n && arr[l] > arr[largest]) {
            largest = l;
        }

        // If right child is larger than largest so far
        if (r < n && arr[r] > arr[largest]) {
            largest = r;
        }

        // If largest is not root
        if (largest != i) {
            int temp = arr[i];
            arr[i] = arr[largest];
            arr[largest] = temp;

            // Recursively heapify the affected sub-tree
            heapify(arr, n, largest);
        }
    }

    // Main function to do heap sort
    static void heapSort(int arr[]) {
        int n = arr.length;

        // Build heap (rearrange array)
        for (int i = n / 2 - 1; i >= 0; i--) {
            heapify(arr, n, i);
        }

        // One by one extract an element from heap
        for (int i = n - 1; i > 0; i--) {

            // Move current root to end
            int temp = arr[0];
            arr[0] = arr[i];
            arr[i] = temp;

            // Call max heapify on the reduced heap
            heapify(arr, i, 0);
        }
    }

    // A utility function to print array of size n
    static void printArray(int arr[]) {
        for (int i = 0; i < arr.length; i++) {
            System.out.print(arr[i] + " ");
        }
        System.out.println();
    }

    // Driver's code
    public static void main(String args[]) {
        int arr[] = {9, 4, 3, 8, 10, 2, 5};
        heapSort(arr);
        System.out.println("Sorted array is ");
        printArray(arr);
    }


```

```java
- Output:
  Sorted array is
  2 3 4 5 8 9 10

```

#### مرتب سازی سریع (quick sort):

```java
import java.util.Arrays;


    // Partition function
    static int partition(int[] arr, int low, int high) {

        // Choose the pivot
        int pivot = arr[high];

        // Index of smaller element and indicates
        // the right position of pivot found so far
        int i = low - 1;

        // Traverse arr[low..high] and move all smaller
        // elements to the left side. Elements from low to
        // i are smaller after every iteration
        for (int j = low; j <= high - 1; j++) {
            if (arr[j] < pivot) {
                i++;
                swap(arr, i, j);
            }
        }

        // Move pivot after smaller elements and
        // return its position
        swap(arr, i + 1, high);
        return i + 1;
    }

    // Swap function
    static void swap(int[] arr, int i, int j) {
        int temp = arr[i];
        arr[i] = arr[j];
        arr[j] = temp;
    }

    // The QuickSort function implementation
    static void quickSort(int[] arr, int low, int high) {
        if (low < high) {

            // pi is the partition return index of pivot
            int pi = partition(arr, low, high);

            // Recursion calls for smaller elements
            // and greater or equals elements
            quickSort(arr, low, pi - 1);
            quickSort(arr, pi + 1, high);
        }
    }

    public static void main(String[] args) {
        int[] arr = {10, 7, 8, 9, 1, 5};
        int n = arr.length;

        quickSort(arr, 0, n - 1);

        for (int val : arr) {
            System.out.print(val + " ");
        }
    }

```

```java
Output
Sorted Array
1 5 7 8 9 10

```

## منابع اضافی:

- [Data Structures Tutorial](https://www.geeksforgeeks.org/data-structures/)
- [Introduction to Data Structures and Algorithms](https://www.w3schools.com/dsa/dsa_intro.php)

## کانال یوتیوب برای آموزش بیشتر:

- [Neon Learn](https://www.youtube.com/@neonlearn)
