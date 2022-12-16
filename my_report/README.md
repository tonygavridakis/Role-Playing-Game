# Lesson: Digital & Serious Games

### First and Last Name: Antonios Gavridakis
### University Registration Number: dpsd19013
### GitHub Personal Profile: https://github.com/tonygavridakis
### Digital & Serious Games Personal Repository: https://tonygavridakis.github.io/Role-Playing-Game/

# Introduction

Στα πλαίσια του μαθήματος Ψηφιακά Παιχνίδια και Παιγνιώδης Μάθηση, καλούμαστε να φτιάξουμε ένα 2D RPG παιχνίδι ως εργασία εξαμήνου.

# Summary


# 1st Deliverable
Αρχικά για τον χαρακτηρα μου μπήκα στο Itch.io στα game assets και έκανα download αυτόν https://seliel-the-shaper.itch.io/character-base
στην συνέχεια εντόπισα το character sprite και έκανα slice κάθε frame του sheet. Έβαλα μέσα στο Scene μου το πρώτο frame και μετα έγραψα τον κώδικα σε C# για να μπορεί να κινείται. Στην συνέχεια κατέβασα ένα TileMap επίσης από το Itch.io (https://cainos.itch.io/pixel-art-top-down-basic), το έκανα slice και έφτιαξα το map μου.
Μετά σε διαφορετικά Tilemaps στο ίδιο Grid έκανα το decorate του Map μου. Στην συνέχεια δημιούργησα ένα Particle System και μετά από αλλαγές στο Emission, το Size και το Size over Lifetime έφτιαξα μια απαλή βροχή. Τέλος για το mood των χρωμάτων μου, έφτιαξα ένα square και του έδωσα ένα transparent χρώμα. 



# 2nd Deliverable
 
 World Interactions - Blocking Movement
 
  Για το blocking movement χρησιμοποίησα διάφορα σχήματα από colliders σαν components σε κάθε αντικείμενο στο tilemap ξεχωριστά διότι με είχαν μπερδέψει στην αρχή τα prefabs και στην συνέχεια με τον ίδιο τρόπο έφτιαξα και colliders περιμετρικά της πίστας για να μην βγαίνει ο χαρακτήρας μου έξω από τα όρια. Μπορέι να μην είναι ακριβώς αυτό που μας λέει να κάνουμε το tutorial, αλλά είναι ένας ακόμα τρόπος να πετύχουμε τον ίδιο σκοπό.
 ![Untitled](https://user-images.githubusercontent.com/101422706/208089716-1f9e75ac-a17b-48f4-a098-1ef57b5a2abe.png)


 World Interactions - Collectibles
 
  Για τα collectibles χρησιμοποίησα αυτό το sprite που βρήκα στο Itch.io στην κατηγορία gameassets:
  ![Food](https://user-images.githubusercontent.com/101422706/208090812-81a33bb0-ff61-48ac-931a-658059536b55.png)
  και από εκεί έκοψα το αντικείμενο που ήθελα να δίνει ζωή στον παίκτη μου και πρόσθεσα τον κώδικα από το tutorial.
  
 World Interactions - Damage Zones and Enemies
 
  Για το επόμενο κομμάτι του παραδοτέου, χρησιμοποίησα τους τάφους που είχα βάλει στο tilemap ως "Damage Zones" ώστε όταν πλησιάζει ο χαρακτήρας να χάνει ζωή, βάζοντάς τους colliders και τον κώδικα του tutorial και δούλεψαν όλα απροβλημάτιστα.
 ![image](https://user-images.githubusercontent.com/101422706/208091475-e141a025-d8f5-4b66-be02-a2da0b609152.png)

Sprite Animation
 
 Στο συγκεκριμένο βήμα, στην αρχή, απλά επικρατούσε το απόλυτο ΧΑΟΣ. Δεν δούλευε με τίποτα, όποιο Tutorial και να ακολουθούσα (Github, Eclass/lab4). Οπότε κατέληξα να βρω την άκρη στο Youtube σε συνδιασμό με δοκιμές που έκανα μόνος μου στα transitions διότι μου κολλούσαν όλα όταν πήγαινα να κουνήσω τον χαρακτήρα από ένα σημείο σε ένα άλλο. Τα sprites του εχθρού που πρόσθεσα σε αυτό το παραδοτέο τα βρήκα επίσης από το Itch.io στην κατηγορία game assets.
 ![AnimationSheet_Character](https://user-images.githubusercontent.com/101422706/208092450-9c412866-9bfc-4743-b202-f5501f103b2e.png)
Επειδή το sprite είναι μόνο προς τα δεξία έκανα animation> Add Properties > Sprite Renderer > Flip X για να γυρνάει από την άλλη πλευρά.
Τέλος με την βοήθεια του Allin1Shader που αναφέρω παρακάτω και μερικών particles που είναι built-in στο Unity, κατάφερα να δώσω ζωή στο map μου κάνοντας animate ΟΛΑ τα χόρτα και τα λουλούδια που υπάρχουν δίνοντας το illusion του άνεμου στην περιοχή που διαδραματίζεται το παιχνίδι.

World Interactions - Projectile

 Ένα ακόμα μέρος της εργασίας που με δυσκόλεψε αρκετά στην αρχή ήταν το κομμάτι των projectiles όμως πάλι μετά από δοκιμές που έκανα μόνος μου αλλά και με το unity package "AllIn1SpriteShader" της εταιρίας Seaside Studios https://assetstore.unity.com/packages/vfx/shaders/all-in-1-sprite-shader-156513, κατάφερα να κάνω τον χαρακτήρα να εκτοξεύει γαλάζιες λάμψεις.
 ![image](https://user-images.githubusercontent.com/101422706/208095513-e61c3d99-91a0-4196-b35a-4ec6f60cdc10.png)

Camera - Cinemachine

 Στην συνέχεια, έκανα install το Cinemachine βάση των οδηγιών του tutorial το οποίο είχα χρησιμοποίσει και στο προιγούμενο παραδοτέο.
 
2D Lighting 

 Τελευταίο πράγμα που πρόσθεσα πριν το ανεβάσω στο profile μου στο Github ήταν ο φωτισμός που προσωπικά πιστεύω ότι έδωσε στο παιχνίδι, ακριβώς την αισθητική που προσπαθούσα να αποδώσω. Μετά από ΠΑΡΑ ΠΟΛΛΑ tutorial στο youtube και 2 βδομαδες ψάξιμο κατάφερα να βρω το "SmartLighting2" της FunkyCode. https://assetstore.unity.com/packages/tools/particles-effects/smart-lighting-2d-112535
![image](https://user-images.githubusercontent.com/101422706/208097215-147ae914-d8f7-4ca4-b80e-4c9766250e91.png)
![image](https://user-images.githubusercontent.com/101422706/208097307-04070166-64a0-45e9-a2d8-323128ea12f9.png)
Έφτιαξα στον χάρτη μου light colliders σε κάθε αντικείμενο που ήθελα να έχει σκιές και μέσα από τα settings του shader ρύθμισα το smoothness των σκιών,τα χρώματα της ατμόσφαιρας, το πόσο δυνατές θα είναι, το πόσο θα επιρεάζονται από την θέση του χαρακτήρα στο map την κάθε στιγμή, αλλά και τα neon χρώματα σε όλες τις επιγραφές πάνω σε βράχους που συναντάμε σε όλο το παιχνίδι. Το shader αυτό ήταν αρκετά βαρύ για να το φορτώσει ο υπολογισής στο εργαστήριο, οπότε το προχώρισα σπίτι μου για να βοηθήσω το unity με μια πιο δυνατή κάρτα γραφικών. 
![image](https://user-images.githubusercontent.com/101422706/208098362-3d5caeb6-87a1-4e5c-b0a4-86484b1a2dc9.png)





# 3rd Deliverable 


# Conclusions


# Sources

https://cainos.itch.io/pixel-art-top-down-basic (ΓΙΑ ΤΟ ΜΑΠ ΜΟΥ)

https://seliel-the-shaper.itch.io/character-base ( ΓΙΑ ΤΟN ΧΑΡΑΚΤΗΡΑ ΜΟΥ)
