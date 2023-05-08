  
  
    //Array codes anlegen
		int[][] codes = getCodes(4);

		// codes ausgeben
		ausgabe(codes);

		// COdes rotieren
		int[][] rotiereCode = rotateright(codes);

		
		ausgabe(rotiereCode);
		
	}

	

	private static int[][] rotateright(int[][] pCodes) {
		// Kopie erstellen
		int[][] copy = pCodes.clone();

		// Array mit rotierten Inhalt erstellen
		int[][] rot = new int[copy.length][copy.length];
		
		//Algorithmus Rotation
		int x2,y2;
		for (int y1 = 0; y1 < rot.length; y1++) {
			for (int x1 = 0; x1 < rot.length; x1++) {
				y2 = x1;
				x2 = 3-y1;
				rot[y2][x2] = copy [y1][x1];
			}
		}
		return rot;
	}

	private static void ausgabe(int[][] codes) {
		for (int y = 0; y < codes.length; y++) {
			for (int x = 0; x < codes.length; x++) {
				System.out.print(codes[y][x] + " ");
			}
			System.out.println("\t");
		}
		System.out.println("----------------------------------------------------------------------------");
	}

	private static int[][] getCodes(int dimension) {
		int[][] c = new int[dimension][dimension];

		int wert =1;
		
		for (int y = 0; y < c.length; y++) {
			for (int x = 0; x < c.length; x++) {
				c[y][x] = wert;
				wert++;
			}
		}

		return c;
	}




Initialisierung:
• Erstelle ein zweidimensionales Integer-Array mit dem Namen "codes" und rufe die Methode "getCodes(4)" auf, um es mit den zurückgegebenen Werten zu befüllen.
• Gib das Array "codes" aus, indem du die Methode "ausgabe(codes)" aufrufst.
• Rufe die Methode "rotateright(codes)" auf, um das Array "codes" um 90 Grad im Uhrzeigersinn zu rotieren und speichere das Ergebnis in einer neuen Variable "rotiereCode".
• Gib das rotierte Array "rotiereCode" aus, indem du die Methode "ausgabe(rotiereCode)" aufrufst.
Methoden:
• Die Methode "rotateright" erhält ein zweidimensionales Integer-Array "pCodes" als Parameter.
• Erstelle eine Kopie von "pCodes" und speichere sie in einem neuen Array "copy".
• Erstelle ein neues Array "rot" mit der gleichen Größe wie "copy".
• Führe eine Schleife aus, die jedes Element in "copy" durchläuft. Verwende die Variable "y1" für die Zeile und "x1" für die Spalte.
• Weise die Werte der Variablen "x2" und "y2" wie folgt zu: "y2" = "x1" und "x2" = 3 - "y1".
• Weise das Element in "copy[y1][x1]" dem Element in "rot[y2][x2]" zu.
• Gib das Array "rot" zurück.
• Die Methode "ausgabe" erhält ein zweidimensionales Integer-Array "codes" als Parameter.
• Führe eine Schleife aus, die jedes Element in "codes" durchläuft. Verwende die Variable "y" für die Zeile und "x" für die Spalte.
• Gib den Wert des Elements in "codes[y][x]" aus.
• Gib am Ende jeder Zeile eine Tabulatorausrichtung aus.
• Gib eine Trennlinie aus.
• Die Methode "getCodes" erhält eine Ganzzahl "dimension" als Parameter.
• Erstelle ein neues zweidimensionales Integer-Array "c" mit "dimension" Zeilen und Spalten.
• Initialisiere eine Variable "wert" mit dem Wert 1.
• Führe eine Schleife aus, die jedes Element in "c" durchläuft. Verwende die Variable "y" für die Zeile und "x" für die Spalte.
• Weise dem Element in "c[y][x]" den Wert "wert" zu und erhöhe "wert" um 1.
• Gib das Array "c" zurück.