int phoneCall(int min1, int min2_10, int min11, int S) {
    int t = 0;
    int i =0;
    if(S >= min1){
        t++;
        S -= min1;
        if(S>= min2_10){
            for(; i < 9 && S>=min2_10; i++){
                t++;
                S-=min2_10;
            }
            if(S>=min11 && i == 9){
                while(S>=min11){
                    t++;
                    S-=min11;
                }
            }
        }
    }
    return t;
}
