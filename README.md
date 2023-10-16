# CITSADM
Esse repositório tem o objetivo de: Todos os envolvidos dasabem! 
///escala 4 tecnicos 

///function updateScale(){

///    let day = new Date();
///    let dayWeek = day.getDay()	

///    if (dayWeek == 5){
///        alert("A escala não pode ser atualizada na sexta-feira.")       
///    } else {
///        listTec = localStorage.getItem('listTec');
///        listTec = JSON.parse(listTec)
    
///        if (listTec.updateScale == 1) {
    
///            tecAudSegAndSexta = listTec.terca
///            tecAudTer = listTec.quarta
///            tecAudQua = listTec.quinta
///            tecAudQui = listTec.segunda
    
///            listTec.segunda = tecAudSegAndSexta
///            listTec.terca = tecAudTer
///            listTec.quarta = tecAudQua
///            listTec.quinta = tecAudQui
///            listTec.updateScale = 0
    
///            if (listTec.corte1 == 'Damiao' || listTec.corte1 == 'Tácio' || listTec.corte1 == 'Tacio' || listTec.corte2 == 'Damiao' || listTec.corte2 == 'Tácio' || listTec.corte2 == 'Tacio') {
///                if (listTec.terca == 'Alisson' || listTec.quarta == 'Mauro') {
///                    listTec.corte1 = 'Mauro';
///                    listTec.corte2 = 'Alisson';
///                } else if (listTec.terca == 'Mauro' || listTec.quarta == 'Alisson') {
///                   listTec.corte1 = 'Alisson';
///                   listTec.corte2 = 'Mauro';
///                } else {
///                    listTec.corte1 = 'Mauro'
///                    listTec.corte2 = 'Alisson'
///                }
///            } else if (listTec.corte1 == 'Alisson' || listTec.corte1 == 'Mauro' || listTec.corte2 == 'Alisson' || listTec.corte2 == 'Mauro') {
///                if (listTec.terca == 'Damiao' || listTec.quarta == 'Tácio' || listTec.quarta == 'Tacio') {
///                    listTec.corte1 = 'Tácio';
///                    listTec.corte2 = 'Damiao';
///               } else if (listTec.terca == 'Tácio' || listTec.terca == 'Tácio' || listTec.quarta == 'Damiao') {
///                    listTec.corte1 = 'Damiao';
///                    listTec.corte2 = 'Tácio';
///                } else {
///                    listTec.corte1 = 'Tácio'
///                    listTec.corte2 = 'Damiao'
///                }
///            }
///            tecCorte1T = listTec.corte1;
///            tecCorte2T = listTec.corte2;
   
///            localStorage.setItem('listTec', JSON.stringify(listTec))
    
///            document.location.reload();
    
///        } else {
///            alert("A escala já foi atualizada esta semana.")
///        }
///    }
///}

/// Função que cria a escala de audiência.
///function audienceScale() {
///    let day = new Date();
///    let dayWeek = day.getDay()	
    
///    if (dayWeek != 5) {
///        if (localStorage.getItem('listTec')) {
///            listTec = localStorage.getItem('listTec');
///            listTec = JSON.parse(listTec)
///            if (listTec.updateScale == 1) {
				 /// Monta a nova escala de AUDIÊNCIA
///                tecAudSegAndSexta = listTec.terca
///                tecAudTer = listTec.quarta
///                tecAudQua = listTec.quinta
///                tecAudQui = listTec.segunda

///                listTec.segunda = tecAudSegAndSexta
///                listTec.terca = tecAudTer
///                listTec.quarta = tecAudQua
///                listTec.quinta = tecAudQui
///                listTec.updateScale = 0

				/// Monta a nova escala da CORTE.
///                if (listTec.corte1 == 'Damiao' || listTec.corte1 == 'Tácio' || listTec.corte1 == 'Tacio' || listTec.corte2 == 'Damiao' || listTec.corte2 == 'Tácio' || listTec.corte2 == 'Tacio') {
///                    if (listTec.terca == 'Alisson' || listTec.quarta == 'Mauro') {
///                       listTec.corte1 = 'Mauro';
///                        listTec.corte2 = 'Alisson';
///                    } else if (listTec.terca == 'Mauro' || listTec.quarta == 'Alisson') {
///                        listTec.corte1 = 'Alisson';
///                        listTec.corte2 = 'Mauro';
///                    } else {
///                        listTec.corte1 = 'Mauro'
///                        listTec.corte2 = 'Alisson'
///                    }
///                } else if (listTec.corte1 == 'Alisson' || listTec.corte1 == 'Mauro' || listTec.corte2 == 'Alisson' || listTec.corte2 == 'Mauro') {
///                    if (listTec.terca == 'Damiao' || listTec.quarta == 'Tácio' || listTec.quarta == 'Tacio') {
///                        listTec.corte1 = 'Tácio';
///                        listTec.corte2 = 'Damiao';
///                    } else if (listTec.terca == 'Tácio' || listTec.terca == 'Tácio' || listTec.quarta == 'Damiao') {
///                        listTec.corte1 = 'Damiao';
///                        listTec.corte2 = 'Tácio';
///                    } else {
///                        listTec.corte1 = 'Tácio'
///                        listTec.corte2 = 'Damiao'
///                    }
///                }
///                tecCorte1T = listTec.corte1;
///                tecCorte2T = listTec.corte2;

///               localStorage.setItem('listTec', JSON.stringify(listTec))
///            } else {
///                tecAudSegAndSexta = listTec.segunda
///                tecAudTer = listTec.terca
///                tecAudQua = listTec.quarta
///                tecAudQui = listTec.quinta
///                tecCorte1T = listTec.corte1;
///                tecCorte2T = listTec.corte2;
///            }
///       }else {
			/// Caso não tenha nenhuma informação de escala no banco.
///            listTec = {'segunda': tecAudSegAndSexta, 'terca': tecAudTer, 'quarta': tecAudQua, "quinta": tecAudQui, "corte1": tecCorte1T, "corte2": tecCorte2T,'updateScale': 1}
///            localStorage.setItem('listTec', JSON.stringify(listTec))
///        }
    
	/// Se for sexta-feira, ele vai informar que a escala precisa ser atualizada. Essa atualização ocorre no próximo dia útil
///    } else if (dayWeek == 5){
///        if (localStorage.getItem('listTec')) {
///            listTec = localStorage.getItem('listTec');
///            listTec = JSON.parse(listTec)

///            tecAudSegAndSexta = listTec.segunda
///            tecAudTer = listTec.terca
///            tecAudQua = listTec.quarta
///            tecAudQui = listTec.quinta
///            tecCorte1T = listTec.corte1;
///            tecCorte2T = listTec.corte2;
///            listTec.updateScale = 1

///            localStorage.setItem('listTec', JSON.stringify(listTec))
///        } else {
			/// Caso não tenha nenhuma informação de escala no banco.
///            if (!localStorage.getItem('listTec')) {
///                listTec = {'segunda': tecAudSegAndSexta, 'terca': tecAudTer, 'quarta': tecAudQua, "quinta": tecAudQui, "corte1": tecCorte1T, "corte2": tecCorte2T, 'updateScale': 1}
///                localStorage['listTec'] = JSON.stringify(listTec)
///            }
///        }       
///    }
///}

/// Monta a escala na página.
///function scaleThePage(scaleExists) {
///    let monday, tuesday, wednesday, thursday, friday, dayScale = "#004e91";

    /// Se a escala já estiver na página, e precisa ser atualizada, ele exclui para acrescentar a nova escala posteriormente
///    if (scaleExists) {
///        var divOld = document.getElementById("escala");
///        if (divOld.parentNode) {
///            divOld.parentNode.removeChild(divOld);
///        }
///    }
///
///    if (dayWeek == 1) {
///        monday = dayScale;
///        tuesday = wednesday = thursday = friday = "none";
///    } else {
///        if (dayWeek == 2) {
///            tuesday = dayScale;
///            monday = wednesday = thursday = friday = "none";
///        } else {
///            if (dayWeek == 3) {
///                wednesday = dayScale;
///                monday = tuesday = thursday = friday = "none";
///            } else {
///                if (dayWeek == 4) {
///                    thursday = dayScale;
///                    monday = wednesday = tuesday = friday = "none";
///                } else {
///                    if (dayWeek == 5) {
///                        friday = dayScale;
///                        monday = wednesday = thursday = tuesday = "none";
///                    }
///                }
///            }
///        }
///    }

    /// Alterar HTML da página para incluir a escala.
///    var divInitial = document.createElement('div');
///    divInitial.setAttribute("id", "escala");

///    divInitial.innerHTML = `
///        <div style="">
///            <table border="1" id="title" style="">
///                <caption>
///                    <div>
///                        <h3>ESCALA DE AUDIÊNCIA</h3>
///                        <button id="updateAudienceScale">
///                            <img src="https://cdn-icons-png.flaticon.com/512/8017/8017201.png " width="30" height="30" alt="" title="" class="img-small">
///                       </button>
///                    </div>
///                </caption>
///                <tr style="">
///                    <td style="background-color: `+monday+`">SEGUNDA</td>
///                    <td style="background-color: `+tuesday+`">TERÇA</td>
///                    <td style="background-color: `+wednesday+`">QUARTA</td>
///                    <td style="background-color: `+thursday+`">QUINTA</td>
///                    <td style="background-color: `+friday+`">SEXTA</td>
///                </tr>
///                <tr>
///                    <td style="background-color: `+monday+`">`+tecAudSegAndSexta+`</td>
///                    <td style="background-color: `+tuesday+`">`+tecAudTer+`</td>
///                    <td style="background-color: `+wednesday+`">`+tecAudQua+`</td>
///                    <td style="background-color: `+thursday+`">`+tecAudQui+`</td>
///                    <td style="background-color: `+friday+`">`+tecAudSegAndSexta+`</td>
///                </tr>
///            </table>
///            <table border="1" id="title" style="">
///                <caption>
///                    <div>
///                        <h3>ESCALA DA CORTE</h3>
///                    </div>
///                </caption>
///                <tr style="">
///                    <td style="background-color: `+tuesday+`">1ª TURMA DE JULGAMENTOS</td>
///                    <td style="background-color: `+wednesday+`">2ª TURMA DE JULGAMENTOS</td>
///                </tr>
///                <tr>
///                    <td style="background-color: `+tuesday+`">`+tecCorte1T+`</td>
///                    <td style="background-color: `+wednesday+`">`+tecCorte2T+`</td>
///                </tr>
///            </table>
///        </div>
///    `

///    document.body.appendChild(divInitial);
///}

///function monitoringScale(){
///    let newDay = new Date();
///    let newDayWeek = newDay.getDay();	

///    if (newDayWeek != dayWeek) {
///        dayWeek = newDayWeek;
///        audienceScale();
///		courtScale();
///        scaleThePage(true);
///    }
///}

///let day = new Date();
///let dayWeek = day.getDay()	
///let tecAudSegAndSexta = "Alisson", tecAudTer = "Tácio", tecAudQua = "Mauro", tecAudQui = "Damiao";
///let tecCorte1T = "Mauro", tecCorte2T = "Alisson"
///let listTec

///audienceScale();
///scaleThePage(false);

///let updateAudienceScale = document.getElementById('updateAudienceScale')
///let updateCorteScale = document.getElementById('updateCorteScale')

///updateAudienceScale.onclick = function() {
///    updateScale()
///}

///setInterval(monitoringScale, 1000); 


///escala 3 tecnicos 


function updateScale(){

    let day = new Date();
    let dayWeek = day.getDay()	

    if (dayWeek == 5){
        alert("A escala não pode ser atualizada na sexta-feira.")       
    } else {
        listTec = localStorage.getItem('listTec');
        listTec = JSON.parse(listTec)
    
        if (listTec.updateScale == 1) {
    
            tecAudSegAndSexta = listTec.terca
            tecAudTer = listTec.quarta
            tecAudQua = listTec.quinta
            tecAudQui = listTec.segunda
    
            listTec.segunda = tecAudSegAndSexta
            listTec.terca = tecAudTer
            listTec.quarta = tecAudQua
            listTec.quinta = tecAudQui
            listTec.updateScale = 0
    
            if (listTec.corte1 == 'Damiao' || listTec.corte1 == 'Tácio' || listTec.corte1 == 'Tacio' || listTec.corte2 == 'Damiao' || listTec.corte2 == 'Tácio' || listTec.corte2 == 'Tacio') {
                if (listTec.terca == 'Alisson' || listTec.quarta == 'Mauro') {
                    listTec.corte1 = 'Mauro';
                    listTec.corte2 = 'Alisson';
                } else if (listTec.terca == 'Mauro' || listTec.quarta == 'Alisson') {
                    listTec.corte1 = 'Alisson';
                    listTec.corte2 = 'Mauro';
                } else {
                    listTec.corte1 = 'Mauro'
                    listTec.corte2 = 'Alisson'
                }
            } else if (listTec.corte1 == 'Alisson' || listTec.corte1 == 'Mauro' || listTec.corte2 == 'Alisson' || listTec.corte2 == 'Mauro') {
                if (listTec.terca == 'Damiao' || listTec.quarta == 'Tácio' || listTec.quarta == 'Tacio') {
                    listTec.corte1 = 'Tácio';
                    listTec.corte2 = 'Damiao';
                } else if (listTec.terca == 'Tácio' || listTec.terca == 'Tácio' || listTec.quarta == 'Damiao') {
                    listTec.corte1 = 'Damiao';
                    listTec.corte2 = 'Tácio';
                } else {
                    listTec.corte1 = 'Tácio'
                    listTec.corte2 = 'Damiao'
                }
            }
            tecCorte1T = listTec.corte1;
            tecCorte2T = listTec.corte2;
    
            localStorage.setItem('listTec', JSON.stringify(listTec))
    
            document.location.reload();
    
        } else {
            alert("A escala já foi atualizada esta semana.")
        }
    }
}

/// Função que cria a escala de audiência.
function audienceScale() {
    let day = new Date();
    let dayWeek = day.getDay();	
    
    if (dayWeek != 5) {
        if (localStorage.getItem('listTec')) {
            listTec = localStorage.getItem('listTec');
            listTec = JSON.parse(listTec);
            
            if (listTec.updateScale == 1) {
                // Monta a nova escala de AUDIÊNCIA
                let availableTechs = ['Mauro', 'Alisson', 'Tácio'];
                
                let audTech1 = availableTechs.shift();
                let audTech2 = availableTechs.shift();
                let audTech3 = availableTechs.shift();
                
                tecAudSegAndSexta = audTech1;
                tecAudTer = audTech2;
                tecAudQua = audTech3;
                
                // Monta a nova escala da CORTE
                if (listTec.corte1 == 'Damiao') {
                    listTec.corte1 = audTech1;
                }
                if (listTec.corte2 == 'Damiao') {
                    listTec.corte2 = audTech1;
                }
                
                listTec.updateScale = 0;
                tecCorte1T = listTec.corte1;
                tecCorte2T = listTec.corte2;
                
                localStorage.setItem('listTec', JSON.stringify(listTec));
            } else {
                tecAudSegAndSexta = listTec.segunda;
                tecAudTer = listTec.terca;
                tecAudQua = listTec.quarta;
                tecAudQui = listTec.quinta;
                tecCorte1T = listTec.corte1;
                tecCorte2T = listTec.corte2;
            }
        } else {
            // Caso não tenha nenhuma informação de escala no banco.
            listTec = {
                'segunda': tecAudSegAndSexta,
                'terca': tecAudTer,
                'quarta': tecAudQua,
                'quinta': tecAudQui,
                'corte1': tecCorte1T,
                'corte2': tecCorte2T,
                'updateScale': 1
            };
            localStorage.setItem('listTec', JSON.stringify(listTec));
        }
    } else if (dayWeek == 5) {
        if (localStorage.getItem('listTec')) {
            listTec = localStorage.getItem('listTec');
            listTec = JSON.parse(listTec);
            
            tecAudSegAndSexta = listTec.segunda;
            tecAudTer = listTec.terca;
            tecAudQua = listTec.quarta;
            tecAudQui = listTec.quinta;
            tecCorte1T = listTec.corte1;
            tecCorte2T = listTec.corte2;
            listTec.updateScale = 1;
            
            localStorage.setItem('listTec', JSON.stringify(listTec));
        } else {
            // Caso não tenha nenhuma informação de escala no banco.
            if (!localStorage.getItem('listTec')) {
                listTec = {
                    'segunda': tecAudSegAndSexta,
                    'terca': tecAudTer,
                    'quarta': tecAudQua,
                    'quinta': tecAudQui,
                    'corte1': tecCorte1T,
                    'corte2': tecCorte2T,
                    'updateScale': 1
                };
                localStorage['listTec'] = JSON.stringify(listTec);
            }
        }
    }
}


/// Monta a escala na página.
function scaleThePage(scaleExists) {
    let monday, tuesday, wednesday, thursday, friday, dayScale = "#004e91";

    /// Se a escala já estiver na página, e precisa ser atualizada, ele exclui para acrescentar a nova escala posteriormente
    if (scaleExists) {
        var divOld = document.getElementById("escala");
        if (divOld.parentNode) {
            divOld.parentNode.removeChild(divOld);
        }
    }

    if (dayWeek == 1) {
        monday = dayScale;
        tuesday = wednesday = thursday = friday = "none";
    } else {
        if (dayWeek == 2) {
            tuesday = dayScale;
            monday = wednesday = thursday = friday = "none";
        } else {
            if (dayWeek == 3) {
                wednesday = dayScale;
                monday = tuesday = thursday = friday = "none";
            } else {
                if (dayWeek == 4) {
                    thursday = dayScale;
                    monday = wednesday = tuesday = friday = "none";
                } else {
                    if (dayWeek == 5) {
                        friday = dayScale;
                        monday = wednesday = thursday = tuesday = "none";
                    }
                }
            }
        }
    }

    /// Alterar HTML da página para incluir a escala.
    var divInitial = document.createElement('div');
    divInitial.setAttribute("id", "escala");

    divInitial.innerHTML = `
        <div style="">
            <table border="1" id="title" style="">
                <caption>
                    <div>
                        <h3>ESCALA DE AUDIÊNCIA</h3>
                        <button id="updateAudienceScale">
                            <img src="https://cdn-icons-png.flaticon.com/512/8017/8017201.png " width="30" height="30" alt="" title="" class="img-small">
                        </button>
                    </div>
                </caption>
                <tr style="">
                    <td style="background-color: `+monday+`">SEGUNDA</td>
                    <td style="background-color: `+tuesday+`">TERÇA</td>
                    <td style="background-color: `+wednesday+`">QUARTA</td>
                    <td style="background-color: `+thursday+`">QUINTA</td>
                    <td style="background-color: `+friday+`">SEXTA</td>
                </tr>
                <tr>
                    <td style="background-color: `+monday+`">`+tecAudSegAndSexta+`</td>
                    <td style="background-color: `+tuesday+`">`+tecAudTer+`</td>
                    <td style="background-color: `+wednesday+`">`+tecAudQua+`</td>
                    <td style="background-color: `+thursday+`">`+tecAudQui+`</td>
                    <td style="background-color: `+friday+`">`+tecAudSegAndSexta+`</td>
                </tr>
            </table>
            <table border="1" id="title" style="">
                <caption>
                    <div>
                        <h3>ESCALA DA CORTE</h3>
                    </div>
                </caption>
                <tr style="">
                    <td style="background-color: `+tuesday+`">1ª TURMA DE JULGAMENTOS</td>
                    <td style="background-color: `+wednesday+`">2ª TURMA DE JULGAMENTOS</td>
                </tr>
                <tr>
                    <td style="background-color: `+tuesday+`">`+tecCorte1T+`</td>
                    <td style="background-color: `+wednesday+`">`+tecCorte2T+`</td>
                </tr>
            </table>
        </div>
    `

    document.body.appendChild(divInitial);
}

function monitoringScale(){
    let newDay = new Date();
    let newDayWeek = newDay.getDay();	

    if (newDayWeek != dayWeek) {
        dayWeek = newDayWeek;
        audienceScale();
		courtScale();
        scaleThePage(true);
    }
}

let day = new Date();
let dayWeek = day.getDay()	
let tecAudSegAndSexta = "Mauro", tecAudTer = "Alisson", tecAudQua = "Tácio", tecAudQui = "Alisson";
let tecCorte1T = "Tácio", tecCorte2T = "Alisson"
let listTec

audienceScale();
scaleThePage(false);

let updateAudienceScale = document.getElementById('updateAudienceScale')
let updateCorteScale = document.getElementById('updateCorteScale')

updateAudienceScale.onclick = function() {
    updateScale()
}

setInterval(monitoringScale, 1000); 
