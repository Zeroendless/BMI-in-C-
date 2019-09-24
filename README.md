+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
+++++++++++++++++++++++++++++Question++++++++++++++++++++++++++++++++
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

Write a program that calculates the user’s body mass index (BMI) and categorizes it as
underweight, normal, overweight or obese, based on the following table from the United States
Centers for Disease Control:

BMI  Weight Status
Below 18.5 Underweight
18.5 – 24.9 Normal
25.0 – 29.9  Overweight
30.0 and above  Obese

To calculate BMI based on the weight in pounds ( wt_lb ) and height in inches ( ht_in ), use this
formula ( round to tenths ):

703 x wt_lb/ht_in 2

Sample Run:

USER’S BODY MASS INDEX (BMI) CALCULATOR
Enter weight in pounds => 600.00
Enter height in inches => 165.50
You BMI is 15.40 and your weight status is underweight.

+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
++++++++++++++++++++++++++++++Answer+++++++++++++++++++++++++++++++++
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

//#include<iostream>//

using namespace std;

int main()
{
	cout<<"USER’S BODY MASS INDEX (BMI) CALCULATOR"<<endl;
	
	float ht_in,wt_lb,bmi;
	cout<<"Enter weight in pounds =>";
	cin>>wt_lb;
	cout<<"Enter height in inches =>";
	cin>>ht_in;
	bmi=703*wt_lb/(ht_in*ht_in);
	
	if(bmi<18.5)
	{
	cout<<"You BMI is"<<bmi<<"and your weight status is underweight.";
    }
	else if(bmi>=18.5 && bmi<=24.9)
	{
	cout<<"You BMI is"<<bmi<<"and your weight status is normal.";
	}
	else if(bmi>=25.0 && bmi<=29.9) 
	{
	cout<<"You BMI is"<<bmi<<"and your weight status is overweight.";
	}
	else
	{
	cout<<"You BMI is"<<bmi<<"and your weight status is obese.";
	}
	
	system("pause"); 
	return 0;
} 


