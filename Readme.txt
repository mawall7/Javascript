- Uppgiften är från https://adriann.github.io/programming_problems.html -> Advanced

- Programmet/scriptet ska jämföra två strängar som innehåller flera 
  substringar med olika längd och slutligen returnera den gemensamt
  längsta substringen.

  Min lösning:

  1. Dela upp strängarna i varsin array; a1 och a2. Skapa också en array för matchningar (tom från början)

  2.  Skapa en array för alla substrängar, vilka som är matchande
      mellan a1 och a2. 
      
      För varje item (forEach) görs en check (isEqual). 
      isEqual använder s2.includes(item) som returnerar 
      endast lika strängar (matchande mellan s1 och s2)
      och i såfall adderar strängelementet till matches.

   3. Kolla slutligen vilken som är den längsta strängen i matches.
      med inbyggda reduce funktionen. som kan gå igenom
      en array och ta argument från det aktuella itemet(a) i en
      array och det tidigare (b) (matches.reduce(function(a, b)){
          villkor för a och b } 
      
      Gör sedan en max check. med max som returnerar det största värdet.
      var longest = matches.reduce(
          function(Total, previousvalue)
          {
              return Math.max(Total.length, currentvalue.length;
          })
      
