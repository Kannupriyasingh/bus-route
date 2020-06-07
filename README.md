# bus-route
question from kick start of round B 2020
   
        #include <iostream>	
        #include <bits/stdc++.h>
        using namespace std;
        int main ()
        { 
            int t;
            long long int x,i,j,n,d;
            cin >> t;		
            for ( i = 0; i < t; i++)
            {
                cin >> n >> d;
                stack < long long int >route;
                for (j = 0; j < n; j++)
	            {
	                cin >> x;
	                route.push (x);
	            }
                while (!route.empty ())
	            {
	                long long int c = route.top ();
	                route.pop ();
	                d = d - d % c;
                }
        cout << "Case #" << i+1 << ": " << d << endl;
        }
        return 0;
        }
