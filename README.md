# Clinique

Personne = (NNI VARCHAR(50), nom VARCHAR(50), prenom VARCHAR(50));
Patient = (IDP VARCHAR(50), CANM VARCHAR(50), #NNI);
Medecin = (IDm VARCHAR(50), specialite VARCHAR(50), #NNI);
Consultation = (IDc VARCHAR(50), dateC DATE, #IDP, #IDm);
Medicament = (codeM VARCHAR(50), libellet VARCHAR(50));
prescrire = (#IDc, #codeM);
