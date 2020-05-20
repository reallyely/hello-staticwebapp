FROM mcr.microsoft.com/azure-cli
RUN apk add --update nodejs npm fish
SHELL ["fish", "-c"]
RUN curl -L https://get.oh-my.fish > install
RUN fish install --path=~/.local/share/omf --config=~/.config/omf --noninteractive
RUN omf install pure && ln -s $OMF_PATH/themes/pure/conf.d/pure.fish ~/.config/fish/conf.d/pure.fish
RUN npm install -g yarn