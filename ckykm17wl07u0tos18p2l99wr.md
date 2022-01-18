## Sliding Window Algorithm

The sliding window technique is used to solve some of the array or string complex problems involving. It reduces Time complexity from *O(n²) to O(n)*.


**Window Sliding Technique Explain**

%[https://www.youtube.com/watch?v=9-3BXsfrpbY&list=PLqM7alHXFySEQDk2MDfbwEdjd2svVJH9p]


**Python Code Example:-
**

```python
# O(n) solution for finding
# maximum sum of a subarray of size k


def maxSum(arr, k):
	# length of the array
	n = len(arr)

	# n must be greater than k
	if n < k:
		print("Invalid")
		return -1

	# Compute sum of first window of size k
	window_sum = sum(arr[:k])

	# first sum available
	max_sum = window_sum

	# Compute the sums of remaining windows by
	# removing first element of previous
	# window and adding last element of
	# the current window.
	for i in range(n - k):
		window_sum = window_sum - arr[i] + arr[i + k]
		max_sum = max(window_sum, max_sum)

	return max_sum


# Driver code
arr = [1, 4, 2, 10, 2, 3, 1, 0, 20]
k = 4
print(maxSum(arr, k))
``` 

**Interview questions used the sliding window technique:-**

<p id="d4f1" class="hi hj ft hk b hl ic hm hn ho id hp hq hr ie hs ht hu if hv hw hx ig hy hz ib do bf" data-selectable-paragraph="">1. <a class="dz iq" href="https://www.techiedelight.com/find-longest-substring-containing-k-distinct-characters/" rel="noopener ugc nofollow" target="_blank">Find the longest substring of a given string containing k distinct characters</a></p><p id="0d32" class="hi hj ft hk b hl ic hm hn ho id hp hq hr ie hs ht hu if hv hw hx ig hy hz ib do bf" data-selectable-paragraph="">2. <a class="dz iq" href="https://www.techiedelight.com/find-substrings-string-permutation-given-string/" rel="noopener ugc nofollow" target="_blank">Find all substrings of a string that are permutation of a given string</a></p><p id="e7da" class="hi hj ft hk b hl ic hm hn ho id hp hq hr ie hs ht hu if hv hw hx ig hy hz ib do bf" data-selectable-paragraph="">3. <a class="dz iq" href="https://www.techiedelight.com/find-longest-substring-given-string-containing-distinct-characters/" rel="noopener ugc nofollow" target="_blank">Longest substring of given string containing distinct characters</a></p><p id="3c99" class="hi hj ft hk b hl ic hm hn ho id hp hq hr ie hs ht hu if hv hw hx ig hy hz ib do bf" data-selectable-paragraph="">4. <a class="dz iq" href="https://www.techiedelight.com/find-maximum-length-sequence-continuous-ones-sliding-window/" rel="noopener ugc nofollow" target="_blank">Find maximum length sequence of continuous ones (Using Sliding Window)</a></p><p id="4bab" class="hi hj ft hk b hl ic hm hn ho id hp hq hr ie hs ht hu if hv hw hx ig hy hz ib do bf" data-selectable-paragraph="">5. <a class="dz iq" href="https://www.techiedelight.com/find-maximum-sequence-of-continuous-1s-can-formed-replacing-k-zeroes-ones/" rel="noopener ugc nofollow" target="_blank">Find the maximum sequence of continuous 1’s that can be formed by replacing at-most k zeroes by ones</a></p><p id="829c" class="hi hj ft hk b hl ic hm hn ho id hp hq hr ie hs ht hu if hv hw hx ig hy hz ib do bf" data-selectable-paragraph="">6. <a class="dz iq" href="https://www.techiedelight.com/find-minimum-sum-subarray-given-size-k/" rel="noopener ugc nofollow" target="_blank">Find minimum sum subarray of given size k</a></p><p id="68e0" class="hi hj ft hk b hl ic hm hn ho id hp hq hr ie hs ht hu if hv hw hx ig hy hz ib do bf" data-selectable-paragraph="">7. <a class="dz iq" href="https://www.techiedelight.com/find-subarray-having-given-sum-given-array/" rel="noopener ugc nofollow" target="_blank">Find subarray having given sum in given array of integers</a></p><p id="7a86" class="hi hj ft hk b hl ic hm hn ho id hp hq hr ie hs ht hu if hv hw hx ig hy hz ib do bf" data-selectable-paragraph="">8. <a class="dz iq" href="https://www.techiedelight.com/length-of-smallest-subarray-with-sum-greater-number/" rel="noopener ugc nofollow" target="_blank">Find the length of the smallest subarray whose sum of elements is greater than the given number</a></p><p id="a4f8" class="hi hj ft hk b hl ic hm hn ho id hp hq hr ie hs ht hu if hv hw hx ig hy hz ib do bf" data-selectable-paragraph="">9. <a class="dz iq" href="https://www.techiedelight.com/count-distinct-elements-every-sub-array-size-k-array/" rel="noopener ugc nofollow" target="_blank">Find the count of distinct elements in every sub-array of size k</a></p><p id="159b" class="hi hj ft hk b hl ic hm hn ho id hp hq hr ie hs ht hu if hv hw hx ig hy hz ib do bf" data-selectable-paragraph="">10. <a class="dz iq" href="https://www.techiedelight.com/print-sub-arrays-array-distinct-elements/" rel="noopener ugc nofollow" target="_blank">Print all sub-arrays of an array having distinct elements</a></p><p id="98a2" class="hi hj ft hk b hl ic hm hn ho id hp hq hr ie hs ht hu if hv hw hx ig hy hz ib do bf" data-selectable-paragraph="">11. <a class="dz iq" href="https://www.techiedelight.com/count-distinct-absolute-values-sorted-array/" rel="noopener ugc nofollow" target="_blank">Count the distinct absolute values in the sorted array</a></p><p id="460d" class="hi hj ft hk b hl ic hm hn ho id hp hq hr ie hs ht hu if hv hw hx ig hy hz ib do bf" data-selectable-paragraph="">12. <a class="dz iq" href="https://www.techiedelight.com/find-duplicates-within-given-range-array/" rel="noopener ugc nofollow" target="_blank">Find duplicates within given range k in an array</a></p><p id="c337" class="hi hj ft hk b hl ic hm hn ho id hp hq hr ie hs ht hu if hv hw hx ig hy hz ib do bf" data-selectable-paragraph=""></p></div>


**Reference:-**

-  [Sliding Window Algorithm](https://www.baeldung.com/cs/sliding-window-algorithm) 



*Thanks for reading.*