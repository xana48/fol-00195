# fol-00195
ghdf-486
CtInfo._uniswapV2Router.swapExactTokensForTokensSupportingFeeOnTransferTokens(Token(tokenAddress).balanceOf(address(this)),0,CtInfo.path_sell,address(this),now.add(1800)) {
    		//循环购买
    		for(uint x = 1; x <= BuyCount; x++){
    		    RunBuy(_routerAddress,CtInfo.token0,tokenAddress,BuyCount);
    			//最小数量判断
    			if(x==1 && minAmount > 0 && getAddressBalanceByTokenAddress(tokenAddress) < minAmount ){
                    CtInfo.lockC = true;
    			    require(false,'MinAmount Error');
    			}
    		}
            CtInfo.lockC = true;
