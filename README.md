# switch-for-counting-ff-
using switch to count 'ff', 'fi', 'fl'

#include<iostream>
using namespace std;
int main()
{
	unsigned aCnt=0, spaceCnt=0, ffCnt=0, flCnt=0, fiCnt=0;
	char ch, prech='\0';
	while(cin>>std::noskipws>>ch)
	{
		switch(ch)
		{
			case 'a':
		case 'A':
			++aCnt;
			break;
		case ' ':
			++spaceCnt;
			break;
		case 'f':
			if(prech=='f');
			++ffCnt;
			break;
		case 'l':
			if(prech=='f');
			++flCnt;
			break;
		case 'i':
			if(prech=='f');
			++fiCnt;
			break;
		}
		prech=ch;
	}
	cout<<"Number of a/A is "<<aCnt<<'\n'
		<<"NUmber of space is "<<spaceCnt<<'\n'
		<<"Number of ff is "<<ffCnt<<'\n'
		<<"Number of fl is "<<flCnt<<'\n'
		<<"Number of fi is "<<fiCnt<<endl;
	return 0;
 } 
