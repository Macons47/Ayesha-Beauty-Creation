# Ayesha-Beauty-Creation

Start
AyeshaBeautyCreation; {
}
if (Already have an account?) {
  Sign in;
} else {
  Sign up 
}
HomePage;
if(Staff?) {
 Enter Authentication;
 Dashboard
} else {;
Customer;
(CustomerDashboard)
End

Start
(Customer Dashboard)
Go to Cart
Cart;
if(Items purchased?) {
  Go to Sales department;
  while(!confirm purchase?)
    Read Order not received;
} Redirect to Sales personnel{
Print virtual receipt;
end;

Budget(budgetTotal){
Set: Products, Price, budgetTotal, Capital
Read: "Products"
Read: "Prices"
Read: "budgetTotal" }

budgetTotal(){
Set: Products
Read: "Products"
Read: "Prices"
Read: "Capital"
budgetTotal="Products" * "Price"
if(budgetTotal<=Capital)then
Print "Budget valid"
    else
Print "Budget Invalid" }

Profit(){
Set: Sales, Expenses
Read: "Sales", "Expenses"
Profit="Sales"-"Expenses"
if(Profit<"Expenses")
Print "Profit Made"
   else
Print "Loss Made"
ENDif }

Application(Age, yearsOFEXperience, Gender){
Set: Age, yearsOFExperience, Gender
Read: "Age"
Read: "yearsOFExperience"
Read: "Gender" }

Age(){ 
if("Age">18)then
Read: yearsOFExperience
    else
Print "Underage"
ENDif }

yearsOFExperience(){
if("yearsOFExperience"==1)then
Read: "Gender"
    else
Print "Minimum 1 year experience required"
ENDif }

Gender(){
if("Gender"=="Female")then
Print "set in queu"
   else
Print "Only females accepted"
ENDif }


Attendance(workHours, breakHours, hoursWorked)
Set: workedHours, breakHours, hoursWorked
Read: workedHours
Read: "breakHours"
Read: "hoursWorked"
Print "hoursWorked" }

workHours(){
Set: startHour, endHour
Read: "startHour"
Read: "endHour"
workHours=endHour-startHour }

breakHours(){
Set: breakStart, breakEnd
Read: "breakStart" 
Read: "breakEnd"
breakHours=breakEnd-breakStart }

hoursWorked(){
Set: breakHours, workHours
Read: breakHours
Read: workHours
hoursWorked=workHours-breakHours }

Expenses(totalExpense){
Set: productCosts, Creditors, Repairs, Electricity, Transport, Water, totalExpense
Read: "Creditors"
Read: "productCosts"
Read: "Expenses"
Read: "Creditors" 
Read: "Repairs" 
Read: "Electricity" 
Read: "Transport" 
Read: "Water"
Read: totalExpense
Print "totalExpense" }

totalExpense(){
Set: productCosts, Creditors, Repairs, Electricity, Transport, Water
Read: "productCosts"
Read: "Creditors" 
Read: "Repairs" 
Read: "Electricity" 
Read: "Transport" 
Read: "Water"
totalExpense="productCosts"+"Creditors"+"Repairs"+"Electricity"+"Transport"+"Water" }


productReports(Solved, solutionInProgress, Unresolved){
Set: Problem, Solved, solutionInProgress, Unresolved
Read: "Problem"
Read: "Solved"
Read: "solutionInProgress"
Read: "Unresolved" }

Solved(){
Set: Problem, solved
Read: "Problem"
Read: "Solved"
if(Problem==Solved)then
Print "Problem has been resolved" 
ENDif }

solutionInProgress(){
Set:Problem, solutionInProgress
Read: "Problem"
Read: "solutionInProgress"
if(Problem==solutionInProgress)then
Print "Problem is yet to be resloved"
ENDif }

Unresolved(){
Set: Problem, Unresolved
Read: Problem
Read: Unresolved
if( Problem==Unresolved)then
Print "Problem remains unresolved"
ENDif }










