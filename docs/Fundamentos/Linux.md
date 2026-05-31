
# **Linux**

Linux é um sistema operacional de código aberto baseado no kernel Linux, criado por Linus Torvalds em 1991. Ele é amplamente utilizado em servidores, desktops, dispositivos móveis e sistemas embarcados devido à sua estabilidade, segurança e flexibilidade. O Linux é conhecido por sua comunidade ativa de desenvolvedores e usuários, que contribuem para o desenvolvimento contínuo do sistema operacional.

# **Comandos úteis para o Linux**


<table style="width: 100%; border-collapse: collapse; font-family: system-ui, -apple-system, sans-serif; font-size: 14px; text-align: left;">
  <thead>
    <tr style="background-color: rgba(128, 128, 128, 0.15); border-bottom: 2px solid rgba(128, 128, 128, 0.5);">
      <th style="padding: 12px 15px; width: 5%;">#</th>
      <th style="padding: 12px 15px; width: 20%;">Comando</th>
      <th style="padding: 12px 15px; width: 75%;">Descrição (Português)</th>
    </tr>
  </thead>
  <tbody>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px; opacity: 0.6;">1</td>
      <td style="padding: 10px 15px;"><code>pwd</code></td>
      <td style="padding: 10px 15px;">Exibe o diretório de trabalho atual.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2); background-color: rgba(128, 128, 128, 0.05);">
      <td style="padding: 10px 15px; opacity: 0.6;">2</td>
      <td style="padding: 10px 15px;"><code>ls</code></td>
      <td style="padding: 10px 15px;">Lista o conteúdo do diretório.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px; opacity: 0.6;">3</td>
      <td style="padding: 10px 15px;"><code>cd</code></td>
      <td style="padding: 10px 15px;">Navega ou altera o diretório atual.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2); background-color: rgba(128, 128, 128, 0.05);">
      <td style="padding: 10px 15px; opacity: 0.6;">4</td>
      <td style="padding: 10px 15px;"><code>mkdir</code></td>
      <td style="padding: 10px 15px;">Cria um novo diretório.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px; opacity: 0.6;">5</td>
      <td style="padding: 10px 15px;"><code>rm</code></td>
      <td style="padding: 10px 15px;">Remove arquivos ou diretórios.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2); background-color: rgba(128, 128, 128, 0.05);">
      <td style="padding: 10px 15px; opacity: 0.6;">6</td>
      <td style="padding: 10px 15px;"><code>cp</code></td>
      <td style="padding: 10px 15px;">Copia arquivos e diretórios.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px; opacity: 0.6;">7</td>
      <td style="padding: 10px 15px;"><code>mv</code></td>
      <td style="padding: 10px 15px;">Move ou renomeia arquivos e diretórios.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2); background-color: rgba(128, 128, 128, 0.05);">
      <td style="padding: 10px 15px; opacity: 0.6;">8</td>
      <td style="padding: 10px 15px;"><code>touch</code></td>
      <td style="padding: 10px 15px;">Cria um arquivo vazio ou atualiza a data/hora de um arquivo existente.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px; opacity: 0.6;">9</td>
      <td style="padding: 10px 15px;"><code>cat</code></td>
      <td style="padding: 10px 15px;">Exibe o conteúdo de um arquivo.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2); background-color: rgba(128, 128, 128, 0.05);">
      <td style="padding: 10px 15px; opacity: 0.6;">10</td>
      <td style="padding: 10px 15px;"><code>head</code></td>
      <td style="padding: 10px 15px;">Exibe as primeiras linhas de um arquivo.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px; opacity: 0.6;">11</td>
      <td style="padding: 10px 15px;"><code>tail</code></td>
      <td style="padding: 10px 15px;">Exibe as últimas linhas de um arquivo.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2); background-color: rgba(128, 128, 128, 0.05);">
      <td style="padding: 10px 15px; opacity: 0.6;">12</td>
      <td style="padding: 10px 15px;"><code>grep</code></td>
      <td style="padding: 10px 15px;">Pesquisa por um padrão de texto em arquivos.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px; opacity: 0.6;">13</td>
      <td style="padding: 10px 15px;"><code>find</code></td>
      <td style="padding: 10px 15px;">Pesquisa por arquivos e diretórios no sistema.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2); background-color: rgba(128, 128, 128, 0.05);">
      <td style="padding: 10px 15px; opacity: 0.6;">14</td>
      <td style="padding: 10px 15px;"><code>tar</code></td>
      <td style="padding: 10px 15px;">Cria ou extrai arquivos do tipo tar (arquivamento).</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px; opacity: 0.6;">15</td>
      <td style="padding: 10px 15px;"><code>gzip</code></td>
      <td style="padding: 10px 15px;">Compacta arquivos.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2); background-color: rgba(128, 128, 128, 0.05);">
      <td style="padding: 10px 15px; opacity: 0.6;">16</td>
      <td style="padding: 10px 15px;"><code>gunzip</code></td>
      <td style="padding: 10px 15px;">Descompacta arquivos compactados com gzip.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px; opacity: 0.6;">17</td>
      <td style="padding: 10px 15px;"><code>zip</code></td>
      <td style="padding: 10px 15px;">Cria ou extrai arquivos compactados em zip.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2); background-color: rgba(128, 128, 128, 0.05);">
      <td style="padding: 10px 15px; opacity: 0.6;">18</td>
      <td style="padding: 10px 15px;"><code>unzip</code></td>
      <td style="padding: 10px 15px;">Extrai o conteúdo de um arquivo zip.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px; opacity: 0.6;">19</td>
      <td style="padding: 10px 15px;"><code>ssh</code></td>
      <td style="padding: 10px 15px;">Conecta a um servidor remoto de forma segura via SSH.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2); background-color: rgba(128, 128, 128, 0.05);">
      <td style="padding: 10px 15px; opacity: 0.6;">20</td>
      <td style="padding: 10px 15px;"><code>scp</code></td>
      <td style="padding: 10px 15px;">Copia arquivos entre máquinas locais e remotas via SSH.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px; opacity: 0.6;">21</td>
      <td style="padding: 10px 15px;"><code>wget</code></td>
      <td style="padding: 10px 15px;">Faz o download de arquivos da web.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2); background-color: rgba(128, 128, 128, 0.05);">
      <td style="padding: 10px 15px; opacity: 0.6;">22</td>
      <td style="padding: 10px 15px;"><code>curl</code></td>
      <td style="padding: 10px 15px;">Transfere dados de ou para um servidor usando diversos protocolos.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px; opacity: 0.6;">23</td>
      <td style="padding: 10px 15px;"><code>man</code></td>
      <td style="padding: 10px 15px;">Exibe o manual de instruções de um comando.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2); background-color: rgba(128, 128, 128, 0.05);">
      <td style="padding: 10px 15px; opacity: 0.6;">24</td>
      <td style="padding: 10px 15px;"><code>which</code></td>
      <td style="padding: 10px 15px;">Exibe o caminho do diretório (localização) de um comando.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px; opacity: 0.6;">25</td>
      <td style="padding: 10px 15px;"><code>history</code></td>
      <td style="padding: 10px 15px;">Exibe o histórico de comandos digitados no terminal.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2); background-color: rgba(128, 128, 128, 0.05);">
      <td style="padding: 10px 15px; opacity: 0.6;">26</td>
      <td style="padding: 10px 15px;"><code>sudo</code></td>
      <td style="padding: 10px 15px;">Executa um comando com privilégios de administrador (root).</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px; opacity: 0.6;">27</td>
      <td style="padding: 10px 15px;"><code>su</code></td>
      <td style="padding: 10px 15px;">Alterna para outra conta de usuário.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2); background-color: rgba(128, 128, 128, 0.05);">
      <td style="padding: 10px 15px; opacity: 0.6;">28</td>
      <td style="padding: 10px 15px;"><code>chmod</code></td>
      <td style="padding: 10px 15px;">Altera as permissões de leitura, escrita e execução de um arquivo/diretório.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px; opacity: 0.6;">29</td>
      <td style="padding: 10px 15px;"><code>chown</code></td>
      <td style="padding: 10px 15px;">Altera o usuário dono de um arquivo ou diretório.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2); background-color: rgba(128, 128, 128, 0.05);">
      <td style="padding: 10px 15px; opacity: 0.6;">30</td>
      <td style="padding: 10px 15px;"><code>chgrp</code></td>
      <td style="padding: 10px 15px;">Altera o grupo proprietário de um arquivo ou diretório.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px; opacity: 0.6;">31</td>
      <td style="padding: 10px 15px;"><code>du</code></td>
      <td style="padding: 10px 15px;">Estima e exibe o espaço em disco ocupado por arquivos e diretórios.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2); background-color: rgba(128, 128, 128, 0.05);">
      <td style="padding: 10px 15px; opacity: 0.6;">32</td>
      <td style="padding: 10px 15px;"><code>df</code></td>
      <td style="padding: 10px 15px;">Exibe o uso de espaço livre e ocupado no disco.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px; opacity: 0.6;">33</td>
      <td style="padding: 10px 15px;"><code>top</code></td>
      <td style="padding: 10px 15px;">Exibe em tempo real o uso de recursos do sistema e os processos rodando.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2); background-color: rgba(128, 128, 128, 0.05);">
      <td style="padding: 10px 15px; opacity: 0.6;">34</td>
      <td style="padding: 10px 15px;"><code>ps</code></td>
      <td style="padding: 10px 15px;">Exibe um instantâneo dos processos atuais em execução.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px; opacity: 0.6;">35</td>
      <td style="padding: 10px 15px;"><code>kill</code></td>
      <td style="padding: 10px 15px;">Encerra ou envia sinais para processos em execução.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2); background-color: rgba(128, 128, 128, 0.05);">
      <td style="padding: 10px 15px; opacity: 0.6;">36</td>
      <td style="padding: 10px 15px;"><code>ifconfig</code></td>
      <td style="padding: 10px 15px;">Configura ou exibe informações das interfaces de rede.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px; opacity: 0.6;">37</td>
      <td style="padding: 10px 15px;"><code>ping</code></td>
      <td style="padding: 10px 15px;">Envia pacotes de teste (ICMP) para um host para testar a conexão de rede.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2); background-color: rgba(128, 128, 128, 0.05);">
      <td style="padding: 10px 15px; opacity: 0.6;">38</td>
      <td style="padding: 10px 15px;"><code>nslookup</code></td>
      <td style="padding: 10px 15px;">Consulta servidores DNS para obter registros de domínio ou IP.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px; opacity: 0.6;">39</td>
      <td style="padding: 10px 15px;"><code>netstat</code></td>
      <td style="padding: 10px 15px;">Exibe conexões de rede, tabelas de roteamento e estatísticas das interfaces.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2); background-color: rgba(128, 128, 128, 0.05);">
      <td style="padding: 10px 15px; opacity: 0.6;">40</td>
      <td style="padding: 10px 15px;"><code>ssh-keygen</code></td>
      <td style="padding: 10px 15px;">Gera pares de chaves pública e privada para autenticação SSH.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px; opacity: 0.6;">41</td>
      <td style="padding: 10px 15px;"><code>awk</code></td>
      <td style="padding: 10px 15px;">Ferramenta de processamento de texto avançada para extrair e manipular dados.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2); background-color: rgba(128, 128, 128, 0.05);">
      <td style="padding: 10px 15px; opacity: 0.6;">42</td>
      <td style="padding: 10px 15px;"><code>sed</code></td>
      <td style="padding: 10px 15px;">Editor de fluxo para transformar ou manipular textos em arquivos.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px; opacity: 0.6;">43</td>
      <td style="padding: 10px 15px;"><code>diff</code></td>
      <td style="padding: 10px 15px;">Compara dois arquivos linha por linha para encontrar diferenças.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2); background-color: rgba(128, 128, 128, 0.05);">
      <td style="padding: 10px 15px; opacity: 0.6;">44</td>
      <td style="padding: 10px 15px;"><code>sort</code></td>
      <td style="padding: 10px 15px;">Ordena as linhas de arquivos de texto.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px; opacity: 0.6;">45</td>
      <td style="padding: 10px 15px;"><code>cut</code></td>
      <td style="padding: 10px 15px;">Remove/extrai seções específicas das linhas de um arquivo.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2); background-color: rgba(128, 128, 128, 0.05);">
      <td style="padding: 10px 15px; opacity: 0.6;">46</td>
      <td style="padding: 10px 15px;"><code>wc</code></td>
      <td style="padding: 10px 15px;">Conta e exibe o número de linhas, palavras e caracteres em um arquivo.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px; opacity: 0.6;">47</td>
      <td style="padding: 10px 15px;"><code>tee</code></td>
      <td style="padding: 10px 15px;">Lê da entrada padrão e grava simultaneamente na saída padrão e em arquivos.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2); background-color: rgba(128, 128, 128, 0.05);">
      <td style="padding: 10px 15px; opacity: 0.6;">48</td>
      <td style="padding: 10px 15px;"><code>uptime</code></td>
      <td style="padding: 10px 15px;">Exibe há quanto tempo o sistema está ligado e as médias de carga.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px; opacity: 0.6;">49</td>
      <td style="padding: 10px 15px;"><code>who</code></td>
      <td style="padding: 10px 15px;">Exibe quais usuários estão atualmente conectados ao sistema.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2); background-color: rgba(128, 128, 128, 0.05);">
      <td style="padding: 10px 15px; opacity: 0.6;">50</td>
      <td style="padding: 10px 15px;"><code>date</code></td>
      <td style="padding: 10px 15px;">Exibe ou permite configurar a data e hora do sistema.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px; opacity: 0.6;">51</td>
      <td style="padding: 10px 15px;"><code>cal</code></td>
      <td style="padding: 10px 15px;">Exibe um calendário no terminal.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2); background-color: rgba(128, 128, 128, 0.05);">
      <td style="padding: 10px 15px; opacity: 0.6;">52</td>
      <td style="padding: 10px 15px;"><code>free</code></td>
      <td style="padding: 10px 15px;">Exibe a quantidade de memória RAM livre e usada no sistema.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px; opacity: 0.6;">53</td>
      <td style="padding: 10px 15px;"><code>uname</code></td>
      <td style="padding: 10px 15px;">Exibe informações básicas do sistema operacional (como versão do kernel).</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2); background-color: rgba(128, 128, 128, 0.05);">
      <td style="padding: 10px 15px; opacity: 0.6;">54</td>
      <td style="padding: 10px 15px;"><code>route</code></td>
      <td style="padding: 10px 15px;">Exibe ou manipula a tabela de roteamento de IP.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px; opacity: 0.6;">55</td>
      <td style="padding: 10px 15px;"><code>iptables</code></td>
      <td style="padding: 10px 15px;">Ferramenta de administração para filtragem de pacotes e NAT (firewall IPv4).</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2); background-color: rgba(128, 128, 128, 0.05);">
      <td style="padding: 10px 15px; opacity: 0.6;">56</td>
      <td style="padding: 10px 15px;"><code>shutdown</code></td>
      <td style="padding: 10px 15px;">Desliga ou reinicia o sistema de forma segura.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px; opacity: 0.6;">57</td>
      <td style="padding: 10px 15px;"><code>reboot</code></td>
      <td style="padding: 10px 15px;">Reinicia (reinicializa) o sistema.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2); background-color: rgba(128, 128, 128, 0.05);">
      <td style="padding: 10px 15px; opacity: 0.6;">58</td>
      <td style="padding: 10px 15px;"><code>halt</code></td>
      <td style="padding: 10px 15px;">Encerra o funcionamento do sistema abruptamente.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px; opacity: 0.6;">59</td>
      <td style="padding: 10px 15px;"><code>locate</code></td>
      <td style="padding: 10px 15px;">Localiza arquivos pelo nome de forma rápida utilizando um banco de dados interno.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2); background-color: rgba(128, 128, 128, 0.05);">
      <td style="padding: 10px 15px; opacity: 0.6;">60</td>
      <td style="padding: 10px 15px;"><code>updatedb</code></td>
      <td style="padding: 10px 15px;">Atualiza o banco de dados de arquivos utilizado pelo comando <code>locate</code>.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px; opacity: 0.6;">61</td>
      <td style="padding: 10px 15px;"><code>alias</code></td>
      <td style="padding: 10px 15px;">Cria um nome alternativo (atalho) para um comando maior ou frequente.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2); background-color: rgba(128, 128, 128, 0.05);">
      <td style="padding: 10px 15px; opacity: 0.6;">62</td>
      <td style="padding: 10px 15px;"><code>source</code></td>
      <td style="padding: 10px 15px;">Executa comandos de um arquivo no ambiente shell atual (ou recarrega configurações).</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px; opacity: 0.6;">63</td>
      <td style="padding: 10px 15px;"><code>crontab</code></td>
      <td style="padding: 10px 15px;">Agenda a execução automática de scripts ou comandos em horários específicos.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2); background-color: rgba(128, 128, 128, 0.05);">
      <td style="padding: 10px 15px; opacity: 0.6;">64</td>
      <td style="padding: 10px 15px;"><code>nohup</code></td>
      <td style="padding: 10px 15px;">Executa um comando que continuará rodando mesmo se o terminal for fechado.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px; opacity: 0.6;">65</td>
      <td style="padding: 10px 15px;"><code>rsync</code></td>
      <td style="padding: 10px 15px;">Sincroniza e transfere arquivos e diretórios de forma rápida entre sistemas.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2); background-color: rgba(128, 128, 128, 0.05);">
      <td style="padding: 10px 15px; opacity: 0.6;">66</td>
      <td style="padding: 10px 15px;"><code>lsof</code></td>
      <td style="padding: 10px 15px;">Lista os arquivos abertos e quais processos estão fazendo uso deles.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px; opacity: 0.6;">67</td>
      <td style="padding: 10px 15px;"><code>lscpu</code></td>
      <td style="padding: 10px 15px;">Exibe informações detalhadas sobre a arquitetura do processador (CPU).</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2); background-color: rgba(128, 128, 128, 0.05);">
      <td style="padding: 10px 15px; opacity: 0.6;">68</td>
      <td style="padding: 10px 15px;"><code>lshw</code></td>
      <td style="padding: 10px 15px;">Exibe informações aprofundadas sobre toda a configuração de hardware.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px; opacity: 0.6;">69</td>
      <td style="padding: 10px 15px;"><code>lspci</code></td>
      <td style="padding: 10px 15px;">Lista e detalha todos os barramentos e dispositivos PCI conectados.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2); background-color: rgba(128, 128, 128, 0.05);">
      <td style="padding: 10px 15px; opacity: 0.6;">70</td>
      <td style="padding: 10px 15px;"><code>lsusb</code></td>
      <td style="padding: 10px 15px;">Lista os barramentos USB e os dispositivos conectados a eles.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px; opacity: 0.6;">71</td>
      <td style="padding: 10px 15px;"><code>iftop</code></td>
      <td style="padding: 10px 15px;">Monitora e exibe em tempo real o uso de largura de banda da rede.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2); background-color: rgba(128, 128, 128, 0.05);">
      <td style="padding: 10px 15px; opacity: 0.6;">72</td>
      <td style="padding: 10px 15px;"><code>sar</code></td>
      <td style="padding: 10px 15px;">Coleta, salva ou emite relatórios sobre diversas atividades do sistema.</td>
    </tr>
    <tr style="border-bottom: 1px solid rgba(128, 128, 128, 0.2);">
      <td style="padding: 10px 15px; opacity: 0.6;">73</td>
      <td style="padding: 10px 15px;"><code>nc</code></td>
      <td style="padding: 10px 15px;">Netcat: um utilitário para ler e escrever dados através de conexões de rede.</td>
    </tr>
  </tbody>
</table>



#### Bibliografia 



#### Histórico de Versões



| Versão |    Data    | Descrição                                 | Autor(es)                                       | Revisor(es)                                    |
| ------ | :--------: | ----------------------------------------- | ----------------------------------------------- | ---------------------------------------------- |
| 1.0    | 30/05/2026 | Criação do documento                        | [Harryson](https://github.com/harry-cmartin) |       |
