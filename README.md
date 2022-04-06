# Receptai
Receptai maisto
class Mokinys{
   String vardasPavarde;
   int[] pazymiai;
   float vidurkis;
   }

   float suma = 0.0F;

Mokinys m1 = new Mokinys();
   m1.vardasPavarde = "Haris Poteris";
   m1.pazymiai = new int[]{8,10,10};


   for (int i=0; i < m1.pazymiai.length; ++i){
   suma +=m1.pazymiai[i];
   }

   m1.vidurkis = suma / m1.pazymiai.length;


Mokinys m2 = new Mokinys();
   m2.vardasPavarde = "Angelina Jolie";
   m2.pazymiai = new int[]{8,7,6};


   for (int i=0; i < m2.pazymiai.length; ++i){
   suma +=m2.pazymiai[i];
   }

   m2.vidurkis = suma / m2.pazymiai.length;


Mokinys m3 = new Mokinys();
   m3.vardasPavarde = "Bruce Lee";
   m3.pazymiai = new int[]{8,7,6};


   for (int i=0; i < m3.pazymiai.length; ++i){
   suma +=m3.pazymiai[i];
   }

   m3.vidurkis = suma / m3.pazymiai.length;


Mokinys m4 = new Mokinys();
   m4.vardasPavarde = "Bruce Lee";
   m4.pazymiai = new int[]{8,7,6};


   for (int i=0; i < m4.pazymiai.length; ++i){
   suma +=m4.pazymiai[i];
   }

   m4.vidurkis = suma / m4.pazymiai.length;


List<Mokinys> mokiniai = new ArrayList();
mokiniai.add(m1);
mokiniai.add(m2);
mokiniai.add(m3);
mokiniai.add(m4);

printArray(mokiniai);

for(Mokinys mok: mokiniai){
  System.out.println("____________________________");
  System.out.println(mok.vardasPavarde);
  System.out.println( nf(mok.vidurkis, 1, 2));
}
// Sukurkite "žurnalą", kuriame surašyti visų mokinių
//vardaiPavardes ir juų vidurkiai.

System.out.println("____________________________");
System.out.println();

Map<string, Float> zurnalas = new HashMap();
for(Mokinys mok: mokiniai){
  zurnalas.put(mok.vardasPavarde,mok.vidurkis);
}
System.out.println(zurnalas);
System.out.println();

//Sukurkite mokinių vidurkių kolekciją ir apskaičiuokite skirtumą
//tarp aukščiausio ir žemiausio vidurkio.

System.out.println("______________Min ir Max vidurkiu skirtumas______________");
System.out.println();

TreeSet<Float> vidurkiai = new TreeSet();
for(Mokinys mok : mokiniai){
  vidurkiai.add(mok.vidurkis);
}
System.out.println(vidurkiai);  
float skirtumas = vidurkiai.last() - vidurkiaifirst();
System.out.println("skirtumas tarp aukščiausio ir žemiausio vidurkio yra " +skirtumas);




