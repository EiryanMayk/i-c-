// portugol

programa
{ 
	inclua biblioteca Util -->d
	funcao inicio ()
	{ 
		// informações 
		inteiro potenciaSangue, idade, cla, vantagens, geracao, idadeMorte, idadeNaoVivo, idadeTotal
		cadeia nome, conceito, comportamento, piorPassado, piorMeu, piorOutros
		inteiro natureza, virtude, vicio, seita
		cadeia Natureza, Virtude, Vicio, Seita
		// demas característica 
		inteiro trilha
		//clans
		inteiro n, rapidez, ofuscacao, quietuz, potencia, presenca, metamorfose, taumaturgia, fortitude, animalismo, serpentis, dominacao, necromancia, tenebrosidade, integridade, quimerismo, vicissitude,  auspicios, demencia 
		inteiro nivelDisciplina1, nivelDisciplina2, nivelDisciplina3
		cadeia	 clan, nomeDisciplina1, nomeDisciplina2, nomeDisciplina3
		// atributos 
		inteiro fisicos, mentais, sociais
		inteiro forca, destreza, vigor, inteligencia, raciocinio, perseveranca, carisma, manipulacao, autocontrole
		// as habilidades 
		inteiro armamento, projeteis, briga, conducao, esportes, furtividade, furto, sobrevivencia, erudicao
		inteiro ciencias, investigacao, medicina, ocultismo, oficios, politica, tecnologia
		inteiro dissimulacao, empatia, expressao, intimidacao, manha, persuasao, socializacao, animais 
		// demas características 
		defesa inteira, deslocamento, iniciativa, tamanho, altura, vitalidade, forçaFontade, fome, vitae
		
		escreva("\t\t->ALERTA!\nPreencha corretamente todos os topicos para uma ficha mais precisa\n")
		escreva("\n->tInfo!!!\n")
		escreva("Algorito para a criação de fichas aleatória nivel 1 de\n")
		escreva("\t\tVampiro a Máscara\n\n") 
		
		escreva("Qual será o nome?\n")
		leia(nome) 
		escreva("Qual será a Altura? NÃO utilize vírgula\n")
		leia(altura) 
		escreva("Pense em um conceito, um esteriótipo para facilitar sua interpretação:\n")
		leia(conceito) 
		escreva("Qual será seu comportamento?\n")
		leia(comportamento)
		//extras 
		escreva("Crie uma erro passado, algo para se arrepender:\n")
		leia(piorPassado)
		escreva("Qual a pior coisa que ele poderia fazer hoje em dia?\n")
		leia(piorMeu)
		escreva("Qual a pior coisa que terceiros poderiam fazer para você?\n")
		leia(piorOutros)
		
		// seitas
		seita = d.sorteia(1,3)
		se ( seita == 1){
			Seita = "Camarilla"
		}se ( seita == 2){
			Seita = "Sabá"
		}se ( seita == 3){
			Seita = "Anarch"
		} 
		// natureza
		natureza = d.sorteia(1,40)
		se ( natureza == 1){
			Natureza = "Advogado do Diabo"
		}se ( natureza == 2){
			Natureza = "Árbitro"
		}se ( natureza == 3){
			Natureza = "Bizarro"
		}se ( natureza == 4){
			Natureza = "Bon Vivant"
		}se ( natureza == 5){
			Natureza = "Caçador"
		}se ( natureza == 6){
			Natureza = "Camaleão"
		}se ( natureza == 7){
			Natureza = "Celebridade"
		}se ( natureza == 8){
			Natureza = "Cientista"
		}se ( natureza == 9){
			Natureza = "Conformista"
		}se ( natureza == 10){
			Natureza = "Criança"
		}se ( natureza == 11){
			Natureza = "Cruzado"
		}se ( natureza == 12){
			Natureza = "Defensor"
		}se ( natureza == 13){
			Natureza = "Ditator"
		}se ( natureza == 14){
			Natureza = "Esperto"
		}se ( natureza == 15){
			Natureza = "Estóico"
		}se ( natureza == 16){
			Natureza = "Exêntrico"
		}se ( natureza == 17){
			Natureza = "Exemplar"
		}se ( natureza == 18){
			Natureza = "Fanático"
		}se ( natureza == 19){
			Natureza = "Filantropo"
		}se ( natureza == 20){
			Natureza = "Galante"
		}se ( natureza == 21){
			Natureza = "Herege"
		}se ( natureza == 22){
			Natureza = "Idealista"
		}se ( natureza == 23){
			Natureza = "Jogador"
		}se ( natureza == 24){
			Natureza = "Juiz"
		}se ( natureza == 25){
			Natureza = "Magnata"
		}se ( natureza == 26){
			Natureza = "Mártir"
		}se ( natureza == 27){
			Natureza = "Masoquista"
		}se ( natureza == 28){
			Natureza = "Melancólico"
		}se ( natureza == 29){
			Natureza = "Pedagogo"
		}se ( natureza == 30){
			Natureza = "Ranzinza"
		}se ( natureza == 31){
			Natureza = "Rebelde"
		}se ( natureza == 32){
			Natureza = "Sádico"
		}se ( natureza == 33){
			Natureza = "Sobrevivente"
		}se ( natureza == 34){
			Natureza = "Sociopata"
		}se ( natureza == 35){
			Natureza = "Soldado"
		}se ( natureza == 36){
			Natureza = "Solitário"
		}se ( natureza == 37){
			Natureza = "Tradicionalista"
		}se ( natureza == 38){
			Natureza = "Valentão"
		}se ( natureza == 39){
			Natureza = "Visionário"
		}se ( natureza == 40){
			Natureza = "Violento"
		}
		// virtudes
		virtude = d.sorteia(1,13)
		se ( virtude == 1){
			Virtude = "Amável"
		}se ( virtude == 2){
			Virtude = "Ambicioso "
		}se ( virtude == 3){
			Virtude = "Confiável"
		}se ( virtude == 4){
			Virtude = "Corajoso"
		}se ( virtude == 5){
			Virtude = "Correto"
		}se ( virtude == 6){
			Virtude = "Esperançoso"
		}se ( virtude == 7){
			Virtude = "Generoso"
		}se ( virtude == 8){
			Virtude = "Honesto"
		}se ( virtude == 9){
			Virtude = "Humilde"
		}se ( virtude == 10){
			Virtude = "Justo"
		}se ( virtude == 11){
			Virtude = "Leal"
		}se ( virtude == 12){
			Virtude = "Paciente"
		}se ( virtude == 13){
			Virtude = "Pacífico"
		} 
		// vicios
		vicio = d.sorteia(1,13)
		se ( vicio == 1){
			Vicio ="Ambicioso"
		}se ( vicio == 2){
			Vicio ="Apresado"
		}se ( vicio == 3){
			Vicio ="Arrogante "
		}se ( vicio == 4){
			Vicio ="Corrupto"
		}se ( vicio == 5){
			Vicio ="Covarte"
		}se ( vicio == 6){
			Vicio ="Cruel"
		}se ( vicio == 7){
			Vicio ="Enganador"
		}se ( vicio == 8){
			Vicio ="Ganancioso "
		}se ( vicio == 9){
			Vicio ="Inconfiável"
		}se ( vicio == 10){
			Vicio ="Odioso"
		}se ( vicio == 11){
			Vicio ="Pessimista "
		}se ( vicio == 12){
			Vicio ="Traiçoeiro"
		}se ( vicio == 13){
			Vicio ="Violento "
		}
		
		idadeMorte = d.sorteia(0,116) 
		idadeNaoVivo = d.sorteia(0,50)
		idadeTotal = idadeMorte + idadeNaoVivo
		// os clãs 
		n = d.sorteia(1,13)
		escolha (n){
			caso 1: //Banu Haqim 
			//rapidez	ofuscação quietuz
			clan = "BANU HAQIM"
			
			rapidez = d.sorteia(1,3)
			ofuscacao = d.sorteia(1,3)
			quietuz = d.sorteia(1,3) 
			enquanto (rapidez == ofuscacao ou rapidez == quietuz){
				rapidez = d.sorteia(1,3)
			}
			enquanto (ofuscacao == quietuz ou ofuscacao == rapidez){
				ofuscacao = d.sorteia(1,3)
			}
			nomeDisciplina3 = "Quietuz"
			nivelDisciplina3 = quietuz 
						
			nomeDisciplina1 = "Rapidez"
			nivelDisciplina1 = rapidez
			 
			nomeDisciplina2 = "Ofuscação"
			nivelDisciplina2 = ofuscacao
			pare 
	
			caso 2: // Brujah 
			//	potencia presenca  rapidez 
			clan = "BRUJAH"	

			rapidez = d.sorteia(1,3)
			potencia = d.sorteia(1,3)
			presenca = d.sorteia(1,3)
			enquanto (rapidez == presenca ou rapidez == potencia){
				rapidez = d.sorteia(1,3)
			}
			enquanto (ofuscacao == presenca ou ofuscacao == rapidez){
				ofuscacao = d.sorteia(1,3)
			}
						
			nomeDisciplina1 = "Rapidez"
			nivelDisciplina1 = rapidez
			 
			nomeDisciplina2 = "Potência"
			nivelDisciplina2 = potencia
			 
			nomeDisciplina3 = "Presença"
			nivelDisciplina3 = presenca
			pare 
			
			caso 3: // Gangrel
			// animalismo fortitude  metamorfose
			
			clan = "GANGREL"	

			metamorfose = d.sorteia(1,3)
			fortitude = d.sorteia(1,3)
			animalismo = d.sorteia(1,3)
			enquanto (metamorfose == fortitude ou metamorfose == animalismo ){
				metamorfose = d.sorteia(1,3)
			}
			quietuz = d.sorteia(1,3)
			enquanto (fortitude == animalismo ou fortitude == metamorfose){
				fortitude = d.sorteia(1,3)
			} 
						
			nomeDisciplina1 = "Animalismo"
			nivelDisciplina1 = animalismo
			 
			nomeDisciplina2 = "Fortitude"
			nivelDisciplina2 = fortitude
			 
			nomeDisciplina3 = "Metamorfose"
			nivelDisciplina3 = metamorfose 
			pare 
			

			caso 4: // Hecata 
			n = d.sorteia(1,5)
			escolha(n){
				caso 1: // Giovanni
					// dominacao potencia  necromancia 
	
				clan = "HECATA/GIOVANNI"	
	
				dominacao = d.sorteia(1,3)
				potencia = d.sorteia(1,3)
				necromancia = d.sorteia(1,3)
				enquanto (dominacao == potencia ou dominacao == necromancia){
					dominacao = d.sorteia(1,3)
				}
				enquanto (potencia == necromancia ou potencia == dominacao){
					potencia = d.sorteia(1,3)
				} 
							
				nomeDisciplina1 = "Rapidez"
				nivelDisciplina1 = rapidez
				 
				nomeDisciplina2 = "Potencia"
				nivelDisciplina2 = potencia
				 
				nomeDisciplina3 = "Necromancia"
				nivelDisciplina3 = necromancia
				pare 
				
				caso 2: // Nagaraja
				// auspicios dominacao necromancia
				clan = "HECATA/NAGARAJA"	
	
				rapidez = d.sorteia(1,3)
				ofuscacao = d.sorteia(1,3)
				presenca = d.sorteia(2,3)
				enquanto (ofuscacao == rapidez ou ofuscacao == quietuz){
					ofuscacao = d.sorteia(1,3)
				}
				enquanto (quietuz == rapidez ou quietuz == ofuscacao){
					quietuz = d.sorteia(1,3)
				} 
							
				nomeDisciplina1 = "Rapidez"
				nivelDisciplina1 = rapidez
				 
				nomeDisciplina2 = "Ofuscação"
				nivelDisciplina2 = ofuscacao
				 
				nomeDisciplina3 = "Presença"
				nivelDisciplina3 = presenca
				pare 
				
				caso 3: // Samedi 
				// fortitude ofuscacao necromancia
				clan = "HECATA/SAMEDI"	
	
				rapidez = d.sorteia(1,3)
				ofuscacao = d.sorteia(1,3)
				presenca = d.sorteia(1,3)
				enquanto (ofuscacao == rapidez ou ofuscacao == quietuz){
					ofuscacao = d.sorteia(1,3)
				}
				enquanto (quietuz == rapidez ou quietuz == ofuscacao){
					quietuz = d.sorteia(1,3)
				} 
							
				nomeDisciplina1 = "Rapidez"
				nivelDisciplina1 = rapidez
				 
				nomeDisciplina2 = "Ofuscação"
				nivelDisciplina2 = ofuscacao
				 
				nomeDisciplina3 = "Presença"
				nivelDisciplina3 = presenca
				pare 
					
				caso 4: //  capadócios
				// auspicios fortitude necromancia
				
				clan = "HECATA/CAPADOCIOS"	
	
				 necromancia = d.sorteia(1,3)
				 fortitude = d.sorteia(1,3)
				 auspicios = d.sorteia(1,3)
				enquanto (necromancia == fortitude ou necromancia == auspicios){
					necromancia = d.sorteia(1,3)
				}
				enquanto (fortitude == auspicios ou fortitude == necromancia){
					fortitude = d.sorteia(1,3)
				} 
							
				nomeDisciplina1 = "Necromancia"
				nivelDisciplina1 = necromancia 
				 
				nomeDisciplina2 = "Fortitude"
				nivelDisciplina2 = fortitude
				 
				nomeDisciplina3 = "Auspícios"
				nivelDisciplina3 = auspicios
				pare 

				pare 

				caso 5: // Lamia 
				// fortitude necromancia  potencia
				clan = "HECATA/LAMIA"
	
				fortitude = d.sorteia(1,3)
				necromancia = d.sorteia(1,3)
				potencia = d.sorteia(1,3)
				enquanto (fortitude == necromancia ou fortitude == potencia){
					fortitude = d.sorteia(1,3)
				}
				enquanto (necromancia == potencia ou necromancia == fortitude){
					necromancia = d.sorteia(1,3)
				}
				nomeDisciplina1 = "Fortitude"
				nivelDisciplina1 = fortitude
				 
				nomeDisciplina2 = "Necromancia"
				nivelDisciplina2 = necromancia 
				 
				nomeDisciplina3 = "Potencia"
				nivelDisciplina3 = potencia
				pare 
			}

			caso 5: // Lasombra 
			// dominacao potencia  tenebrosidade
			clan = "LASOMBRA"

			dominacao = d.sorteia(1,3)
			potencia = d.sorteia(1,3)
			tenebrosidade = d.sorteia(1,3)
			enquanto (dominacao == potencia ou dominacao == tenebrosidade){
				dominacao = d.sorteia(1,3)
			}
			enquanto (potencia == tenebrosidade ou potencia == dominacao){
				potencia = d.sorteia(1,3)
			} 
			nomeDisciplina1 = "Dominação"
			nivelDisciplina1 = dominacao
			 
			nomeDisciplina2 = "Potência"
			nivelDisciplina2 = potencia
			 
			nomeDisciplina3 = "Tenebrosidade"
			nivelDisciplina3 = tenebrosidade
			pare 
			
			caso 6: // Malkavian
			integridade = 5
			// auspicios ofuscacao demencia
			clan = "MALKAVIAN"

			auspicios = d.sorteia(1,3)
			ofuscacao = d.sorteia(1,3)
			demencia = d.sorteia(1,3)
			enquanto ( auspicios == ofuscacao ou auspicios == demencia){
				auspicios = d.sorteia(1,3)
			}
			enquanto (ofuscacao == demencia ou auspicios == ofuscacao){
				ofuscacao = d.sorteia(1,3)
			} 
			nomeDisciplina1 = "Auspicios"
			nivelDisciplina1 = auspicios
			 
			nomeDisciplina2 = "Ofuscação"
			nivelDisciplina2 = ofuscacao
			 
			nomeDisciplina3 = "Demência"
			nivelDisciplina3 = demencia
			pare 
			
			caso 7: // Ministério 
			// ofuscacao presenca  serpentis
			clan = "MINISTÉRIO"	

			serpentis = d.sorteia(1,3)
			ofuscacao = d.sorteia(1,3)
			presenca = d.sorteia(1,3)
			enquanto (ofuscacao == presenca ou ofuscacao == serpentis){
				ofuscacao = d.sorteia(1,3)
			}
			enquanto (serpentis == presenca ou serpentis == ofuscacao){
				serpentis = d.sorteia(1,3)
			} 
			nomeDisciplina1 = "Serpentis"
			nivelDisciplina1 = serpentis
			 
			nomeDisciplina2 = "Ofuscação"
			nivelDisciplina2 = ofuscacao
			 
			nomeDisciplina3 = "Presença"
			nivelDisciplina3 = presenca
			pare 
			
			caso 8: // Nosferatu
			//animalismo potencia  ofuscacao
			clan = "NOSFERATU"	

			animalismo = d.sorteia(1,3)
			potencia = d.sorteia(1,3)
			ofuscacao = d.sorteia(1,3)
			enquanto (ofuscacao == animalismo ou ofuscacao == potencia){
				ofuscacao = d.sorteia(1,3)
			}
			enquanto (animalismo == potencia ou animalismo == ofuscacao){
				animalismo = d.sorteia(1,3)
			} 
			nomeDisciplina1 = "Animalismo"
			nivelDisciplina1 = animalismo
			 
			nomeDisciplina2 = "Ofuscação"
			nivelDisciplina2 = ofuscacao
			 
			nomeDisciplina3 = "Potencia"
			nivelDisciplina3 = potencia
			pare 

			caso 9: // Ravnos
			// animalismo fortitude  quimerismo
			clan = "RAVNOS"

			animalismo = d.sorteia(1,3)
			fortitude = d.sorteia(1,3)
			quimerismo = d.sorteia(1,3)
			enquanto (quimerismo == fortitude ou quimerismo == animalismo){
				quimerismo = d.sorteia(1,3)
			}
			enquanto (fortitude == animalismo ou fortitude == quimerismo){
				fortitude = d.sorteia(1,3)
			} 
			nomeDisciplina1 = "Animalismo"
			nivelDisciplina1 = animalismo
			 
			nomeDisciplina2 = "Fortitude"
			nivelDisciplina2 = fortitude
			 
			nomeDisciplina3 = "Quimerismo"
			nivelDisciplina3 = quimerismo
			pare 
			
			caso 10: // Toreador
			// auspicios rapidez  presenca
			clan = "TOREADOR"

			rapidez = 1
			auspicios = d.sorteia(2,3)
			presenca = d.sorteia(2,3)
			enquanto (auspicios == presenca){
				auspicios = d.sorteia(2,3) 
				presenca = d.sorteia(2,3)
			}
			nomeDisciplina1 = "Rapidez"
			nivelDisciplina1 = rapidez
			 
			nomeDisciplina2 = "Auspicios"
			nivelDisciplina2 = auspicios
			 
			nomeDisciplina3 = "Presença"
			nivelDisciplina3 = presenca
			pare 
			
			caso 11: // Tremere
			// auspicios Dominacao taumaturgia
			clan = "TREMERE"	

			auspicios = d.sorteia(1,3)
			dominacao = d.sorteia(1,3)
			taumaturgia = d.sorteia(1,3)
			enquanto (auspicios == dominacao  ou auspicios == taumaturgia){
				auspicios = d.sorteia(1,3)
			}
			enquanto (dominacao == taumaturgia ou dominacao == auspicios){
				dominacao = d.sorteia(1,3)
			} 
			nomeDisciplina1 = "Auspicios"
			nivelDisciplina1 = auspicios
			 
			nomeDisciplina2 = "Dominação"
			nivelDisciplina2 = dominacao 
			 
			nomeDisciplina3 = "Taumatirgia"
			nivelDisciplina3 = taumaturgia
			pare 
			
			caso 12: // Tzimisce
			// animalismo auspicios vicissitude
			clan = "TZIMISCE"

			animalismo = d.sorteia(1,3)
			auspicios = d.sorteia(1,3)
			vicissitude = d.sorteia(1,3)
			enquanto (animalismo == auspicios ou animalismo == vicissitude){
				animalismo = d.sorteia(1,3)
			}
			enquanto (auspicios == animalismo ou auspicios == vicissitude){
				auspicios = d.sorteia(1,3)
			} 
			nomeDisciplina1 = "Animalismo"
			nivelDisciplina1 = animalismo
			 
			nomeDisciplina2 = "Auspicios"
			nivelDisciplina2 = auspicios
			 
			nomeDisciplina3 = "Vicissitude"
			nivelDisciplina3 = vicissitude
			pare 
		
			caso 13: // Ventrue
			// dominacao fortitude presenca
			clan = "VENTRUE"	

			dominacao = d.sorteia(1,3)
			fortitude = d.sorteia(1,3)
			presenca = d.sorteia(1,3)
			enquanto (dominacao == fortitude ou dominacao == presenca){
				dominacao = d.sorteia(1,3)
			}
			enquanto (fortitude == presenca ou fortitude == presenca){
				fortitude = d.sorteia(1,3)
			} 
			nomeDisciplina1 = "Dominação"
			nivelDisciplina1 = dominacao
			 
			nomeDisciplina2 = "Fortitude"
			nivelDisciplina2 = fortitude
			 
			nomeDisciplina3 = "Presença"
			nivelDisciplina3 = presenca
			pare 
		}
		geracao = 12
		potenciaSangue = 1
		// altura 
		se ( altura >= 200){
			tamanho = 6
		} se ( altura < 200 e altura > 164){
			tamanho = 5
		} se ( altura < 165 e altura > 129){
			tamanho= 4
		} se ( altura < 130 e altura > 94){
			tamanho = 3
		} se ( altura < 95 e altura > 59){
			tamanho = 2
		} se ( altura < 60 e altura > 24){
			tamanho = 1
		} se ( altura < 25){
			tamanho = 0
		} 
		//atributos 
		fisicos = d.sorteia(1,3)
		mentais = d.sorteia(1,3)
		sociais = d.sorteia(1,3)
		// confirmação 
		enquanto (fisicos == mentais ou fisicos == sociais){
			fisicos = d.sorteia(1,3)
		}enquanto(mentais == sociais ou mentais == fisicos){
			mentais = d.sorteia(1,3)
		}
		// físicos 
		se (fisicos == 1){ //5
			forca = d.sorteia(0,5)
			destreza = d.sorteia(0,5)
			vigor = d.sorteia(0,5) 
			
			enquanto ( forca + vigor + destreza != 5 ){
				forca = d.sorteia(0,5)
				destreza = d.sorteia(0,5)
				vigor = d.sorteia(0,5) 
			}
		}se (fisicos == 2){ //4
			forca = d.sorteia(0,4)
			destreza = d.sorteia(0,4)
			vigor = d.sorteia(0,4) 
			
			enquanto ( forca + vigor + destreza != 4 ){
				forca = d.sorteia(0,4)
				destreza = d.sorteia(0,4)
				vigor = d.sorteia(0,4) 
			}
		}se (fisicos == 3){ //3
			forca = d.sorteia(0,3)
			destreza = d.sorteia(0,3)
			vigor = d.sorteia(0,3) 
			
			enquanto ( forca + vigor + destreza != 3 ){
				forca = d.sorteia(0,3)
				destreza = d.sorteia(0,3)
				vigor = d.sorteia(0,3) 
			}
		}
		//mentais
		se (mentais == 1){ //5
			inteligencia = d.sorteia(0,5)
			raciocinio = d.sorteia(0,5)
			perseveranca = d.sorteia(0,5) 
			
			enquanto ( inteligencia + raciocinio + perseveranca != 5 ){
				inteligencia = d.sorteia(0,5)
				raciocinio = d.sorteia(0,5)
				perseveranca = d.sorteia(0,5) 
			}
		}se (mentais == 2){ //4
			inteligencia = d.sorteia(0,4)
			raciocinio = d.sorteia(0,4)
			perseveranca = d.sorteia(0,4) 
			
			enquanto ( inteligencia + raciocinio + perseveranca != 4 ){
				inteligencia = d.sorteia(0,4)
				raciocinio = d.sorteia(0,4)
				perseveranca = d.sorteia(0,4) 
			}
		}se (mentais == 3) { //3
			inteligencia = d.sorteia(0,3)
			raciocinio = d.sorteia(0,3)
			perseveranca = d.sorteia(0,3) 
			
			enquanto ( inteligencia + raciocinio + perseveranca != 3 ){
				inteligencia = d.sorteia(0,3)
				raciocinio = d.sorteia(0,3)
				perseveranca = d.sorteia(0,3) 
			}
		} 
		//sociais
		se (sociais == 1){ //5
			carisma = d.sorteia(0,5)
			manipulacao = d.sorteia(0,5)
			autocontrole = d.sorteia(0,5) 
			
			enquanto ( carisma + manipulacao + autocontrole != 5 ){
				carisma = d.sorteia(0,5)
				manipulacao = d.sorteia(0,5)
				autocontrole = d.sorteia(0,5) 
			}
		}se (sociais == 2){ //4
			carisma = d.sorteia(0,4)
			manipulacao = d.sorteia(0,4)
			autocontrole = d.sorteia(0,4) 
			
			enquanto ( carisma + manipulacao + autocontrole != 4 ){
				carisma = d.sorteia(0,4)
				manipulacao = d.sorteia(0,4)
				autocontrole = d.sorteia(0,4) 
			}
		}se (sociais == 3){ //3
			carisma = d.sorteia(0,3)
			manipulacao = d.sorteia(0,3)
			autocontrole = d.sorteia(0,3) 
			
			enquanto ( carisma + manipulacao + autocontrole != 3 ){
				carisma = d.sorteia(0,3)
				manipulacao = d.sorteia(0,3)
				autocontrole = d.sorteia(0,3) 
			}
		}
		// as habilidades	
		// físicos 
		se (fisicos == 1){ //11
			armamento = d.sorteia(0,11)
			projeteis = d.sorteia(0,11)
			briga = d.sorteia(0,11) 
			conducao = d.sorteia(0,11)
			esportes = d.sorteia(0,11)
			furtividade = d.sorteia(0,11) 
			furto = d.sorteia(0,11)
			sobrevivencia = d.sorteia(0,11)

			enquanto ( armamento + projeteis + briga + conducao + esportes + furtividade + furto + sobrevivencia != 11 ){ 
				armamento = d.sorteia(0,11)
				projeteis = d.sorteia(0,11)
				briga = d.sorteia(0,11) 
				conducao = d.sorteia(0,11)
				esportes = d.sorteia(0,11)
				furtividade = d.sorteia(0,11) 
				furto = d.sorteia(0,11)
				sobrevivencia = d.sorteia(0,11)
			}
		}
		se (fisicos == 2){ //7
			armamento = d.sorteia(0,7)
			projeteis = d.sorteia(0,7)
			briga = d.sorteia(0,7) 
			conducao = d.sorteia(0,7)
			esportes = d.sorteia(0,7)
			furtividade = d.sorteia(0,7) 
			furto = d.sorteia(0,7)
			sobrevivencia = d.sorteia(0,7)

			enquanto ( armamento + projeteis + briga + conducao + esportes + furtividade + furto + sobrevivencia != 7 ){ 
				armamento = d.sorteia(0,7)
				projeteis = d.sorteia(0,7)
				briga = d.sorteia(0,7) 
				conducao = d.sorteia(0,7)
				esportes = d.sorteia(0,7)
				furtividade = d.sorteia(0,7) 
				furto = d.sorteia(0,7)
				sobrevivencia = d.sorteia(0,7)
			}
		}
		se (fisicos == 3){ // 4
			armamento = d.sorteia(0,4)
			projeteis = d.sorteia(0,4)
			briga = d.sorteia(0,4) 
			conducao = d.sorteia(0,4)
			esportes = d.sorteia(0,4)
			furtividade = d.sorteia(0,4) 
			furto = d.sorteia(0,4)
			sobrevivencia = d.sorteia(0,4)

			enquanto ( armamento + projeteis + briga + conducao + esportes + furtividade + furto + sobrevivencia != 4 ){ 
				armamento = d.sorteia(0,1)
				projeteis = d.sorteia(0,4)
				briga = d.sorteia(0,4) 
				conducao = d.sorteia(0,4)
				esportes = d.sorteia(0,4)
				furtividade = d.sorteia(0,4) 
				furto = d.sorteia(0,4)
				sobrevivencia = d.sorteia(0,4)
			}
		}
		//mentais
		se (mentais == 1){ //11
			ciencias = d.sorteia(0,11)
			erudicao = d.sorteia(0,11)
			investigacao = d.sorteia(0,11) 
			medicina = d.sorteia(0,11)
			ocultismo  = d.sorteia(0,11)
			oficios = d.sorteia(0,11) 
			politica = d.sorteia(0,11)
			tecnologia = d.sorteia(0,11)
			
			enquanto ( ciencias + erudicao + investigacao + medicina + ocultismo + oficios + politica + tecnologia != 11 ){ 
				ciencias = d.sorteia(0,11)
				erudicao = d.sorteia(0,11)
				investigacao = d.sorteia(0,11) 
				medicina = d.sorteia(0,11)
				ocultismo  = d.sorteia(0,11)
				oficios = d.sorteia(0,11) 
				politica = d.sorteia(0,11)
				tecnologia = d.sorteia(0,11)
			}
		}
		se (mentais == 2){ //7
			ciencias = d.sorteia(0,7)
			erudicao = d.sorteia(0,7)
			investigacao = d.sorteia(0,7) 
			medicina = d.sorteia(0,7)
			ocultismo  = d.sorteia(0,7)
			oficios = d.sorteia(0,7) 
			politica = d.sorteia(0,7)
			tecnologia = d.sorteia(0,7)
			
			enquanto ( ciencias + erudicao + investigacao + medicina + ocultismo + oficios + politica + tecnologia != 7 ){ 
				ciencias = d.sorteia(0,7)
				erudicao = d.sorteia(0,7)
				investigacao = d.sorteia(0,7) 
				medicina = d.sorteia(0,7)
				ocultismo  = d.sorteia(0,7)
				oficios = d.sorteia(0,7) 
				politica = d.sorteia(0,7)
				tecnologia = d.sorteia(0,7)
			}
		}
		se (mentais == 3) { //4
			ciencias = d.sorteia(0,4)
			erudicao = d.sorteia(0,4)
			investigacao = d.sorteia(0,4) 
			medicina = d.sorteia(0,4)
			ocultismo  = d.sorteia(0,4)
			oficios = d.sorteia(0,4) 
			politica = d.sorteia(0,4)
			tecnologia = d.sorteia(0,4)
			
			enquanto ( ciencias + erudicao + investigacao + medicina + ocultismo + oficios + politica + tecnologia != 4 ){ 
				ciencias = d.sorteia(0,4)
				erudicao = d.sorteia(0,4)
				investigacao = d.sorteia(0,14) 
				medicina = d.sorteia(0,4)
				ocultismo  = d.sorteia(0,4)
				oficios = d.sorteia(0,4) 
				politica = d.sorteia(0,4)
				tecnologia = d.sorteia(0,4)
			}
		} 
		//sociais
		se (sociais == 1){ //11 
		dissimulacao = d.sorteia(0,11)
		empatia = d.sorteia(0,11)
		expressao = d.sorteia(0,11) 
		intimidacao = d.sorteia(0,11)
		manha = d.sorteia(0,11)
		persuasao = d.sorteia(0,11) 
		socializacao = d.sorteia(0,11)
		animais = d.sorteia(0,11)
			
		enquanto ( dissimulacao + empatia + expressao + intimidacao + manha + persuasao + socializacao + animais != 11 ){ 
			dissimulacao = d.sorteia(0,11)
			empatia = d.sorteia(0,11)
			expressao = d.sorteia(0,11) 
			intimidacao = d.sorteia(0,11)
			manha = d.sorteia(0,11)
			persuasao = d.sorteia(0,11) 
			socializacao = d.sorteia(0,11)
			animais = d.sorteia(0,11)
			}
		}
		se (sociais == 2){ //7
		dissimulacao = d.sorteia(0,7)
		empatia = d.sorteia(0,7)
		expressao = d.sorteia(0,7) 
		intimidacao = d.sorteia(0,7)
		manha = d.sorteia(0,7)
		persuasao = d.sorteia(0,7) 
		socializacao = d.sorteia(0,7)
		animais = d.sorteia(0,7)
			
		enquanto ( dissimulacao + empatia + expressao + intimidacao + manha + persuasao + socializacao + animais != 7 ){ 
			dissimulacao = d.sorteia(0,7)
			empatia = d.sorteia(0,7)
			expressao = d.sorteia(0,7) 
			intimidacao = d.sorteia(0,7)
			manha = d.sorteia(0,7)
			persuasao = d.sorteia(0,7) 
			socializacao = d.sorteia(0,7)
			animais = d.sorteia(0,7)
			}
		}
		se (sociais == 3){ //4
		dissimulacao = d.sorteia(0,4)
		empatia = d.sorteia(0,4)
		expressao = d.sorteia(0,4) 
		intimidacao = d.sorteia(0,4)
		manha = d.sorteia(0,4)
		persuasao = d.sorteia(0,4) 
		socializacao = d.sorteia(0,4)
		animais = d.sorteia(0,4)
			
		enquanto ( dissimulacao + empatia + expressao + intimidacao + manha + persuasao + socializacao + animais != 4 ){ 
			dissimulacao = d.sorteia(0,4)
			empatia = d.sorteia(0,4)
			expressao = d.sorteia(0,4) 
			intimidacao = d.sorteia(0,4)
			manha = d.sorteia(0,4)
			persuasao = d.sorteia(0,4) 
			socializacao = d.sorteia(0,4)
			animais = d.sorteia(0,4)
			}
		}
		// demas características  
		se (raciocinio > destreza){
		defesa = raciocinio + esportes 
		} senao{
			defesa = destreza + esportes
		}
		
		deslocamento = forca + tamanho + destreza
		iniciativa = destreza + autocontrole 
		vitalidade = vigor + tamanho
		forcaFontade = perseveranca + autocontrole
		integridade = 7
		trilha = 7
		vitae = d.sorteia(1,10) 
		
		fome = d.sorteia(1,10) 
		se (fome == 1 ou fome == 2){
			fome = 1
		} se (fome == 3 ou fome == 2){
			fome = 2
		} se (fome == 5 ou fome == 6){
			fome = 3
		} se (fome == 7 ou fome == 8){
			fome = 4
		} se (fome == 9 ou fome == 10){
			fome = 5
		} 
		
		limpa()
		escreva("\t\t->Dados Pessoais","\n")
		escreva("Seu nome é:", nome, "\n")
		escreva("Idade: ", idadeMorte, "/", idadeNaoVivo, "/", idadeTotal, "\n")
		escreva("Altura: ", altura, "\n")
		escreva("Conceito: ", conceito, "\n") 
		escreva("Natureza: ", Natureza, "\n")
		escreva("Comportamento: ", comportamento, "\n")
		escreva("Virtude: ", Virtude, "\n")
		escreva("Deslocamento: ", deslocamento, "\n")
		escreva("Vício: ", Vicio, "\n\n")
		escreva("Seu clã é: ",clan,"\n")
		escreva("Seita: ", Seita, "\n")
		escreva("Geração: ", geracao, "\n")
		escreva("Potencia: ", potenciaSangue,"\n")
		escreva("Vitae: ", vitae, "\n")
		escreva("Fome: ", fome,"\n\n")
		
		escreva("\t\t->Suas Disciplinas são:\n")
		escreva(nomeDisciplina1," ",nivelDisciplina1,"\n", nomeDisciplina2, " ", nivelDisciplina2, "\n", nomeDisciplina3," ",nivelDisciplina3,"\n")
		
		escreva ("\t\t->Seus atributos são:\n")
		escreva ("\t Físicos \t Mentais \t Sociais\n")
		escreva ("Força: ",forca + 1 , "\t Inteligência: ",inteligencia + 1, "\tCarisma: ", carisma + 1,"\n")
		escreva ("Destreza: ",destreza + 1,"\t Raciocínio: ",raciocinio + 1, "\t\tManipulação: ", manipulacao + 1,"\n")
		escreva ("Vigor: ",vigor + 1, "\t Perseverança: ", perseveranca + 1, "\tAutocontrole: ", autocontrole + 1,"\n\n")
		
		escreva ("\t\t->Suas Habilidades são:\n")
		escreva ("Armamento: ", armamento,"\t Ciências: ", ciencias, "\t Dissimulação: ", dissimulacao,"\n")
		escreva ("Projéteis: ", projeteis,"\t Erudição: ", erudicao, "\t Empatia: ", empatia,"\n")
		escreva ("Briga: ", briga, "\t\t Investigação: ", investigacao, " Expressão: ", expressao,"\n")
		escreva ("Condução: ", conducao,"\t\t Medicina: ", medicina ,"\t Intimidação:", intimidacao,"\n")
		escreva ("Esportes : ", esportes ,"\t Ocultismo: ", ocultismo ,"\t Manha: ", manha,"\n")
		escreva ("Furtividade: ", furtividade,"\t Oficios: ", oficios ,"\t\t Persuasão:", persuasao,"\n")
		escreva ("Furto: ", furto ,"\t\t Política: ", politica, "\t Socialização: ", socializacao,"\n")
		escreva ("Sobrevivência: ", sobrevivencia," Tecnologia: ", tecnologia ,"\t Trato de Animais: ", animais,"\n\n")
		
		escreva(" \n\n\n")
		escreva("Se deseja acresentar Vantagens e Desvantagens aguarde a seguda versão\n")

		escreva("Baseado na versão alterada de 'Vampiro a Mascara 5'","\n")
		escreva("Para maiores informações ler o pdf:'xxxx' \nou entrar em contato com o dev: eiryanMayk \n")

	}
}
