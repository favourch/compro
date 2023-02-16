# Compro Java code

Answers:
Answer 1:
   <p>Code:</p>
    <pre><code>public static int allValuesTheSame(int[] a) {
    if (a.length == 0) {
        return 0;
    }
    int first = a[0];
    for (int i = 1; i < a.length; i++) {
        if (a[i] != first) {
            return 0;
        }
    }
    return 1;
}</code></pre>

Answer 2:
<p>Code:</p>
    <pre><code>public static boolean hasNValues(int[] a, int n) {
    if (a.length == 0 || n < 1) {
        return false;
    }
    Set<Integer> uniqueValues = new HashSet<>();
    for (int i = 0; i < a.length; i++) {
        uniqueValues.add(a[i]);
        if (uniqueValues.size() > n) {
            return false;
        }
    }
    return true;
}</code></pre>
