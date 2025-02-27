# cost-of-goods
#include <iostream>
#include <iomanip>

using namespace std;

int main () {
			
			int candy, chocolate, mint;
			float candyCost, chocolateCost, mintCost;
			float cost_of_packaging;
			double cost_of_package_process;
			double cost_of_overheads;
			float lossPercent;
			float ingredientCost;
			float cost_oneGiftbox;
			double ingredientLoss;
			double totalCost;
			float sellingPrice;
			float vat;
			float profit_per_box, profit_boxes, vat_boxes;
			int count;
			int selling_Price_Trial;
			
			
						/*
						PROMPT THE USER FOR THE (BULK) COST PER KILOGRAM OF EACH INGREDIENT.
						*/
			
			cout << "Please enter the cost of Candy per kilogram: $";
			cin >> candyCost;
			cout << "Please enter the cost of Chocolate per kilogram: $";
			cin >> chocolateCost;
			cout << "Please enter the cost of Mint per kilogram: $";
			cin >> mintCost;
			cout <<endl;
			
			
						/*
		    			 CALCULATE THE TOTAL COST TO PRODUCE A GIFT BOX.
						*/
			
			cout<< fixed<<setprecision (2);
			
		    /*
			Ingredient Quantity:
			*/
			
			candy = 0.5;
			chocolate = 0.035;
			mint = 0.015;
			
			/*
			 Additional cost associated with producing the gift boxes :
			*/
		
			cost_of_packaging = 0.45;
			cost_of_package_process = 210.00;
			cost_of_overheads = 325.00;
			lossPercent = 0.05;
			
			ingredientCost =candyCost * 0.05 + chocolateCost *0.035 +mintCost *0.015;
			
			cost_oneGiftbox =ingredientCost  + cost_of_packaging + ((cost_of_package_process + cost_of_overheads)/1000)+ lossPercent * ingredientCost;
			
					
			cout << "Cost to produce one gift box : $" <<cost_oneGiftbox <<endl;
			cout <<endl;
			
			
							/*
							DISPLAY A BREAKDOWN OF THE COST TO PRODUCE 1000 GIFT BOXES.
							*/
							
			candy = 0.05;
			chocolate = 0.035;
			mint = 0.015;
			
			cost_of_packaging = cost_of_packaging * 1000;
			ingredientCost =candyCost * 0.05 + chocolateCost *0.035 +mintCost *0.015;
			ingredientLoss = (ingredientCost *0.05 )*1000 ;
			totalCost = ingredientCost*1000 + ingredientLoss + cost_of_packaging + cost_of_package_process + cost_of_overheads;
			
			cout << "Cost breakdown for producing 1000 gift boxes" <<endl;
			cout << "--------------------------------------------" <<endl;
			cout <<endl;
			cout << "Ingredient costs" <<endl;									              //ingredient costs			
			cout << "      Candy            : " <<candyCost * 0.05 *1000<<endl;  
			cout << "      Chocolate        : " <<chocolateCost * 0.035 *1000 <<endl;
			cout << "      Mint             : " <<mintCost *0.015*1000 <<endl;
			cout << "Packaging costs        : " <<cost_of_packaging <<endl;                //packaging costs
			cout << "Packaging process costs: " <<cost_of_package_process <<endl;         //packing process cost 
			cout << "Overhead costs         : " <<cost_of_overheads<<endl;               //overhead cost 
			cout << "Cost due to loss       : " <<ingredientLoss<<endl;                 //costs due to loss of ingredients
			cout << "Total Cost             : " <<totalCost <<endl;                    // total cost
			cout << endl;
		
		
						/*
	    				PROMT THE USER FOR A SELLING PRICE PER BOX.
						*/
			
			 count= 1;
		 
			for(int i = 0; i <3; i++) {
				selling_Price_Trial = selling_Price_Trial + count;
				cout<<endl;
				
				cout << "Selling Price Trial #" << selling_Price_Trial<<endl;
				cout <<endl;
				cout << "Please enter a potential Selling Price: $";
				cin >> sellingPrice;
				cout <<endl;
				
			
				vat = 0.125 * sellingPrice;                                   //VAT of 12.5% added to the selling price
				profit_per_box =sellingPrice- cost_oneGiftbox;               //profit per box
				profit_boxes = profit_per_box * 1000;                       //total profit for 1000 boxes
				vat_boxes = vat * 1000;                                    // VAT for 1000 boxes
			
				
				cout << "Selling price per box            : " <<sellingPrice<<endl;
				cout << "Selling price per box (with VAT) : " <<sellingPrice *0.125 + sellingPrice<<endl;
				cout << "Profit per box                   : " <<profit_per_box <<endl;
				cout << "Profit per 1000 boxes            : " <<profit_boxes <<endl;
				cout << "VAT collected per 1000 boxes     : " <<vat_boxes <<endl;
				
			}
		
			return 0;
		}
			
			
