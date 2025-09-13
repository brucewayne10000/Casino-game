#include <iostream>
#include <ctime>
#include <cstdlib>
#include <bits/stdc++.h>
using namespace std;
int balance {0};
int generatNumber(){
    srand(time(0));
    int randomNum {rand()%4};
   return randomNum;
}
int addMoney(){
    return balance + 100;
}
int takeMoney(){
    return balance - 100;
}
int main(){
    int playersNumber;
    int casinoNumber{generatNumber()};
    int casinoNewNumber2{generatNumber()},casinoNewNumber3{generatNumber()},casinoNewNumber4{generatNumber()};
    cout << "=======================Welcome to Sams Casino,guess the number to win a $100 dollars each right guess!=======================" << endl;
    cout << "current balance $ " << balance << endl;
    cout << "pick a number between 0 and 3:";
    cin >> playersNumber;
    if(playersNumber == casinoNumber){
     balance = addMoney();
      cout << "good guess! you just won some money, this is your current balance: $" << balance << endl;
      cout << "would you like to guess again to get more money(type yes or no)?: ";
      string playersChoice;
      cin >> playersChoice;
      if(playersChoice == "yes"){
        cout << "your a ballsy one huh? guess a number again between 0 and 3: "; 
        int playersNewNumber;
        cin >> playersNewNumber;
            if(playersNewNumber == casinoNewNumber2){
                balance = addMoney();
                cout << "you just won again! this is your current balance $" << balance << endl;
                cout << "this is your third round, pick a number between 0 and 3:";
                cin >> playersNumber;
                    if(playersNumber == casinoNewNumber3){
                    balance = addMoney();
                    cout << " congrats you won again! your current balandce is $" << balance << endl;
                    cout << "this is the last round good luck! pick a number between 0 and 3: ";
                    cin >> playersNumber;
                    if(playersNumber == casinoNewNumber3){
                    balance = addMoney();
                    cout << "==============YOU WON==================" << endl;
                    cout << "GGs you won the game congratulations! your ending balance is $" << balance << endl;
                    }else{
                        balance = takeMoney();
                        cout << "=====================game has ended=========================" << endl;
                    cout << "you lost this is where the round ends. your current balance is" << balance;
                    }
                      }else{
                    balance = takeMoney();
                    cout << "=====================game has ended=========================" << endl;
                    cout << "you lost this is where the round ends. your current balance is" << balance;
                    }
            }else if (playersNewNumber != casinoNewNumber2){
                balance = takeMoney();
               cout << "=====================game has ended=========================" << endl;
                cout << " you just lost $100 dollars current balance is $" << balance;
            }
      }else{
        cout << "the game has ended congrats on your winnings come back next time!";
      }
    }else if (playersNumber != casinoNumber){
        cout << "=====================game has ended=========================" << endl;
        cout << "you lost";
    }
}
