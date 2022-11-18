
# MATCHING-PATTERN



#include <stdio.h>
#include <stdlib.h>
int stockmerchant(int arr[], int n) {
    int freq[100],  ans=0, i;
    for(i=0; i<n; i++)
    {
        freq[arr[i]]++;
    }
    for(int i=0; i<100; i++)
    {
        ans=ans+freq[i]/2;
    }
    return ans;
}
int main()
{
    int n;
    scanf("%d", &n);
    int arr[101], i;
    for(i=0; i<n; i++)
    {
        scanf("%d", &arr[i]);
    }
    int ans=stockmerchant(n, arr);
    printf("%d", ans);
    return 0;
    
}
