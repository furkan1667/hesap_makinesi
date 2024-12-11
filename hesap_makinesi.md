actor hesap_makinesi {   
  var hucre: Int=0;

  
  public func toplama(s:Int): async Int {       //Bu fonksiyon içerisinde toplama işlemleri yapılmaktadır.
    hucre += s;
    hucre
    //(Debug.print(debug_show (hucre));)
  };
  
  public func cikarma(s: Int) : async Int{      //Bu fonksiyon içerisinde çıkarma işlemleri yapılmaktadır.
    hucre -= s;
    hucre
  };
  
  public func carpma(s: Int) : async Int{      //Bu fonksiyon içerisinde çarpma işlemleri yapılmaktadır.
    hucre *= s;
    hucre
  };
  
  public func bolme(s: Int) : async ?Int{     //Bu fonksiyon içerisinde bölmeişlemleri yapılmaktadır.
    if( s==0){            //Bu satırda eğer s değerimiz 0 ise çıkacak değeri null olarak gösterdik.
      null
    }
    else{                 //Bu satırda ise s değerimiz 0 değil ise bölme işlemi yapmaktayız.
      hucre /= s;
      ?hucre
    }
  };

 
  public func temizle(): async(){   //Bu kısımda ise yaptığımız ve bulduğumuz sonuçları temizleme işlemleri yapmaktayız.
    hucre := 0;
  };
}
