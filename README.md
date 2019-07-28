# CodeFunDo2019
A project as a part of the hackathon CodeFunDo 2019


Idea:
      Create an application which uses azure blockchain to record votes and make the record public so that everybody is able to check and verify the votes' correctness.
      
      Advantages:
                Vote can be casted from anywhere.
                Records are public and therefore forgery is not easy.
               
Implementation:
                Use the voterID to generate an unique key whose generating functction is not made public.
                The voter's vote is also encrypted and concatenated with the key generated.
                The constituency id is also concatenated along to generate the final key.
                This key is then stored in the record and broadcasted.
                The person is provided with the final key and can search for the key in the record anytime before the election is over.
                At the time of counting the counting commity is provided with only the votecode and constituency code to maintain anonymity.
