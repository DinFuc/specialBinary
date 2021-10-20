long long specialBinary(long long n)
{
    vector<long long>a{0, 1};
    long long res0 = 0, res1 = 1, pow0 = 2, pow1 = 4;
    for(int i = 0; i < 62; i++){
        if(i & 1){
        res1 += pow1;
        pow1 <<= 2;
        a.push_back(res1);
        }
        else{
            res0 += pow0;
            pow0 <<= 2;
            a.push_back(res0);
        }
    }
    sort(a.begin(), a.end());
    for(long long i : a)
        if(i >= n)
            return i;
}
