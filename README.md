public String without2(String str) {
  
  String answerString = "";

  if(str.length() == 2){
    answerString += "";
  }
  
  else if(str.length() == 3){
    if((str.charAt(0) == str.charAt(1)) && str.charAt(1) == str.charAt(2)){
      answerString += str.charAt(0);
    }
  }
  
  else if(str.length()>=4 && str.substring(0,2).equals(str.substring(str.length()-2))){
    answerString += str.substring(2);
  }
  
  else{
    answerString = str;
  }
  
  return answerString;

}
