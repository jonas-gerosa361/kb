# Soap
** Padrão de mensagem utilizado para XML **
"Soap está para XML assim como Rest está para JSON"
SOAP mantem a URI, o que muda é a soap message

## Estrutura de uma mensagem SOAP
<soap:Envelope xmlns:soap="http://www.w3.org/2003/05-soap-envelope">
    <soap:Header>
    </soap:Header>
    <soap:Body>
        <m:MetodoEndereço xmlns:m="http://www.example.org/endereco">
            <m:Cidade>Rio de Janeiro</m:Cidade>
            <m:CEP>99999-99</m:CEP>
        </m:Endereco>
    </soap:Body>
</soap:Envelope>

## WSDL - Web Services Description Languague (XML)
** Usado para descrever Web Services, funciona como um contrato de serviço **

## XSD - XML Schema Definition
** Schame no formato XML usado para definir a estrutura de dados que será validada no XML **