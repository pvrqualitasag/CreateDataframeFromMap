#include <Rcpp.h>
using namespace Rcpp;

// This is a simple example of exporting a C++ function to R. You can
// source this function into an R session using the Rcpp::sourceCpp 
// function (or via the Source button on the editor toolbar). Learn
// more about Rcpp at:
//
//   http://www.rcpp.org/
//   http://adv-r.had.co.nz/Rcpp.html
//   http://gallery.rcpp.org/
//

// [[Rcpp::export]]
NumericVector timesTwo(NumericVector x) {
  return x * 2;
}

//' Create a Dataframe Using Rcpp
//' 
//' This is the example from Seamless R and C++ from page 55.
// [[Rcpp::export]]
DataFrame create_dataframe() {
  IntegerVector v = IntegerVector::create(7,8,9);
  std::vector<std::string> s(3);
  s[0] = "x";
  s[1] = "y";
  s[2] = "z";
  return DataFrame::create(Named("a") = v,
                           Named("b") = s);
}

// You can include R code blocks in C++ files processed with sourceCpp
// (useful for testing and development). The R code will be automatically 
// run after the compilation.
//

/*** R
timesTwo(42)
*/
